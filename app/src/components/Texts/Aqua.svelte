<script>
    let { text, className = "text-xl text-aqua font-bold @xl:text-2xl @2xl:text-2xl" } = $props();
</script>

<p class={className}>{text}</p>