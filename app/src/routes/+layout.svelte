<script lang="ts">
	import '../app.css';
	import '@fontsource/lemon';
	import '@fontsource-variable/roboto';
	import Footer from '../components/Footer/Footer.svelte';
	import Header from '../components/Header/Header.svelte';
	let { children } = $props();
</script>

<div class="text-main text-sm">
	<Header />
	{@render children()}
	<Footer />
</div>