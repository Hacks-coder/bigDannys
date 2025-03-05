<script>
	import Fill from "../Buttons/Fill.svelte";
	import Aqua from "../Texts/Aqua.svelte";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
</script>
<section class="@container mt-20 px-5">
    <div class="flex flex-col items-center gap-10 @3xl:flex-row @3xl:gap-15 @3xl:justify-center">
        <div class="space-y-2 @3xl:space-y-5 @3xl:w-200">
            <Aqua text = "ANALYTICS" />
            <Title text = "Airtime Top-up with Bonus." />
            <Small text = "Use our built-in analytics dashboard to gain valuable insights and track the performance of your data sales over time. Monitor revenue, customer trends, and market demand to optimize your strategy and maximize profits." />
            <Fill text = "VIEW OUR PRICING" />
        </div>
        <div class="bg-cover bg-center">
            <img src="/others/analysis1.png" alt="" class="size-100 @md:size-120 @2xl:size-150 @4xl:size-170">
        </div>
    </div>
</section>