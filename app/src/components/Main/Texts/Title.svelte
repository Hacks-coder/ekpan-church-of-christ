<script>
    let {text, className = "text-black font-bold text-xl @md:text-2xl @xl:text-3xl @3xl:text-5xl" } = $props();
</script>

<p class={className}>{text}</p>