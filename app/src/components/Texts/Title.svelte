<script>
    let {text, className = "text-2xl font-bold font-title @md:text-3xl @2xl:text-5xl @4xl:text-6xl"} = $props();
</script>


<p class={className}>{text}</p>