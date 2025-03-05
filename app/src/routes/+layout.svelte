<script lang="ts">
	import '../app.css';
	import Footer from '../components/Footer/Footer.svelte';
	import Header from '../components/Header/Header.svelte';
	let { children } = $props();
</script>
<Header />
{@render children()}
<Footer />
