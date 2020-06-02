<svelte:head>
  <style src="../style/global.scss"></style>
</svelte:head>

<script>
	import Nav from '../components/Nav.svelte';
	import Footer from '../components/Footer.svelte'

	export let segment;
</script>

<Nav {segment}/>

<main>
	<slot></slot>
</main>

<Footer />