<script>
	import '$lib/styles/app.css'
</script>

<svelte:head>
	<link
		rel='preconnect'
		href='https://fonts.googleapis.com'
	>
	<link
		rel='preconnect'
		href='https://fonts.gstatic.com'
		crossorigin
	>
	<link
		href='https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@500;900&display=swap'
		rel='stylesheet'
	>
</svelte:head>

<div class='app'>
	<slot></slot>
</div>

<style>
  .app {
    height: 100vh;
  }
</style>
