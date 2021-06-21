<template>
	<div class="row">
		<h3 class="fw-bold mb-3">Why VueJS</h3>
		<div class="col-12 col-md-4">
			<h4 class="fw-bold">Approachable</h4>
			<p>Already know HTML, CSS and JavaScript? Read the guide and start building things in no time!</p>
		</div>
		<div class="col-12 col-md-4">
			<h4 class="fw-bold">Versatile</h4>
			<p>An incrementally adoptable ecosystem that scales between a library and a full-featured framework.</p>
		</div>
		<div class="col-12 col-md-4">
			<h4 class="fw-bold">Performant</h4>
			<p>20KB min+gzip Runtime Blazing Fast Virtual DOM Minimal Optimization Efforts</p>
		</div>
		<div class="alert p-3 text-center my-5" :class="$root.theme == 'darkMode' ? 'alert-light' : 'alert-dark'">
			The learning curve for Vue is a lot less steep than React or Angular in my opinion. I'm biased because I use Vue a lot now, but
			it took me less than a week to get comfortable with Vue+Vuex. I tried Angular a lot before and it never felt anything like as
			natural or enjoyable as Vue. I think React is great but I don't find it as fun (personal preference).
		</div>
	</div>
</template>

<script>
	module.exports = {
		name: 'home',
	};
</script>

<style scoped></style>
