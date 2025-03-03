<script>
    import IconFacebook from '~icons/mdi/facebook';
    import IconYoutube from '~icons/mdi/youtube';
    import IconInstagram from '~icons/mdi/instagram';
    import IconMail from '~icons/mdi/email'; 

    const mediaLinks = [
        {icon: IconFacebook},
        {icon: IconYoutube},
        {icon: IconInstagram},
        {icon: IconMail},
    ]
</script>

<nav class="flex gap-2">
    {#each mediaLinks as {icon}}
        <a href="/" class="text-gold text-2xl"><svelte:component this={icon} /></a>
    {/each}
</nav>