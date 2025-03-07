<script lang="ts">
	import '../app.css';
	import '@fontsource/lemon';
	import '@fontsource-variable/roboto';
	import Footer from '../components/Footer/Footer.svelte';
	import Header from '../components/Header/Header.svelte';
	import Hero from '../components/Main/StaticDirs/Hero.svelte';
	let { children } = $props();
</script>

<div class="text-main text-sm">
	<Header />
	<Hero />
	{@render children()}
	<Footer />
</div>