<script>
    let { text, className = "text-lg text-aqua font-bold @xl:text-xl @2xl:text-2xl" } = $props();
</script>

<p class={className}>{text}</p>