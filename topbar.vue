<template>
	<div class="d-flex justify-content-end my-3">
		<div class="form-check form-switch">
			<input @click="toggleTheme" class="form-check-input" type="checkbox" id="flexSwitchCheckDefault" />
			<label v-if="this.$root.theme == 'darkMode'" class="form-check-label" for="flexSwitchCheckDefault"> Light </label>
			<label v-else class="form-check-label" for="flexSwitchCheckDefault"> Dark </label>
		</div>
	</div>
</template>

<script>
	module.exports = {
		name: 'topbar',
		methods: {
			toggleTheme() {
				//toggles theme value
				this.$root.theme = this.$root.theme == 'darkMode' ? '' : 'darkMode';
				// sets the data-theme attribute
				document.documentElement.setAttribute('data-theme', this.$root.theme);
				// stores theme value on local storage
				localStorage.setItem('theme', this.$root.theme);
			},
		},
	};
</script>

<style scoped>
	label:hover {
		cursor: pointer;
	}
</style>
