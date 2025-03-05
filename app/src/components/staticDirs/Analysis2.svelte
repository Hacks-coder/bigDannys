<script>
	import Fill from "../Buttons/Fill.svelte";
	import Aqua from "../Texts/Aqua.svelte";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
</script>
<section class="@container mt-20 px-5">
    <div class="flex flex-col items-center gap-10 @3xl:flex-row @3xl:gap-15 @3xl:justify-center">
        <div class="bg-cover bg-center order-2 @3xl:order-0">
            <img src="/others/analysis2.png" alt="" class="size-100 @md:size-120 @2xl:size-150 @4xl:size-170">
        </div>
        <div class="space-y-2 @3xl:space-y-5 @3xl:w-200">
            <Aqua text = "ANALYTICS" />
            <Title text = "Data Top-up with Bonus.." />
            <Small text = "Don't miss out on our extreme data bonuses! We’ve got you covered with the best prices and unbeatable deals, ensuring you get more data for less. Whether you're streaming, browsing, or working online, our generous offers guarantee seamless connectivity without breaking the bank." />
            <Fill text = "VIEW OUR PRICING" />
        </div>
    </div>
</section>