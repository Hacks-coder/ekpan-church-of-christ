<script>
    let {text, className = "text-black font-bold text-lg @md:text-xl @2xl:text-2xl @4xl:text-4xl" } = $props();
</script>

<p class={className}>{text}</p>