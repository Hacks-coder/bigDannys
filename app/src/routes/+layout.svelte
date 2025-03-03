<script lang="ts">
	import '../app.css';
	let { children } = $props();
	import '@fontsource-variable/roboto';
	import '@fontsource/konkhmer-sleokchher';
	import Header from '../components/staticDirs/Header.svelte';
	import SubFooter from '../components/Footer/SubFooter.svelte';
</script>
<div class="@container text-black font-main overflow-hidden flex flex-col min-h-screen gap-5 xl:gap-30">
	<Header />
	<main class="flex-1">{@render children()}</main>
	<SubFooter />
</div>
