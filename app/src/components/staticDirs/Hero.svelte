<script>
	import Fill from "../Buttons/Fill.svelte";
	import Outline from "../Buttons/Outline.svelte";
	import Small from "../Texts/Small.svelte";

	
    const photo = "/others/hero.png"

</script>
<section class="@container">
    <div class="grid gap-10 place-items-center pl-10 pr-10 @3xl:grid-cols-2">
        <div class="space-y-3">
            <div class="space-y-3">
                <p class="bg-gradient-to-r from-purple to-gold bg-clip-text text-transparent font-bold text-4xl font-title @xl:text-5xl @2xl:text-6xl @4xl:text-8xl">Buy Airtime & Data Anywhere</p>
                <Small text = "The most secure marketplace for buying and selling unique crypto assets." />
            </div>
            <div class="flex gap-2">
                <Fill text = "Buy Data" />
                <Outline text = "Sell Data" />
            </div>
        </div>
        <div style={`background-image: url(${photo})`} class="bg-cover bg-center size-80 @md:size-100 @xl:size-120 @4xl:size-120 @5xl:size-170"></div>
    </div>
</section>