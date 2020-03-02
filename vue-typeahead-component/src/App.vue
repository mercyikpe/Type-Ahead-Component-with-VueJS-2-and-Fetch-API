<template>
	<div id="app">
		<div class="Wrap text-center">
			<h1>Vue Typeahead</h1>
			<p>Simple VueJS 2 TypeAhead component built with Fetch Browser API.</p>

			<!-- Our component-->
			<typeahead
				source="https://jsonplaceholder.typicode.com/posts"
				placeholder="What TV Series you are looking for..."
				filter-key="title"
				:start-at="2"
			>
			</typeahead>
		</div>
	</div>
</template>

<script>

	import Typeahead from './components/Typeahead.vue'

	export default {

		name: 'app',

		components: { Typeahead  }

	}

</script>

<style>
	body {
		margin: 0; padding: 0;
		font-family: 'Open Sans', Arial, sans-serif;
		box-sizing: border-box;
		background: linear-gradient(135deg, #41B883 0%,#354953 100%);
		background-size: cover;
		min-height: 100vh;
		color: #fff;
	}
	h1 {
		font-size: 6vw;
	}
	h1, h2, h3, h4 {
		margin: 0; padding: 0;
		font-family: 'Lobster', Arial, sans-serif;
	}
	.text-center {
		text-align: center;
	}
	.Wrap {
		max-width: 60vw;
		margin: 15vh auto;
	}
</style>
