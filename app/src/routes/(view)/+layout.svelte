<script lang="ts">
	import Footer from '../../components/Footer/Footer.svelte';
import Hero from '../../components/staticDirs/Hero.svelte';

	let { children } = $props();
</script>
<Hero />
{@render children()}
<Footer />