<script lang="ts">
	import Hero from '../../components/Main/StaticDirs/Hero.svelte';


	let { children } = $props();
</script>

<div class="text-main text-sm">
	<Hero />
	{@render children()}
</div>