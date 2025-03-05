<script>
    import LightbulbOnOutline from '~icons/mdi/lightbulb-on-outline';
    import ShieldCheck from '~icons/mdi/shield-check';
    import CurrencyUsd from '~icons/mdi/currency-usd';
    import Headset from '~icons/mdi/headset';
    import AccountCircle from '~icons/mdi/account-circle';
    import Flash from '~icons/mdi/flash';
	import Small from '../Texts/Small.svelte';

    const services = [
        {
            icon: LightbulbOnOutline,
            title: "Innovativeness",
            description: "We constantly introduce new features and improvements to enhance user experience and provide cutting-edge solutions for data and airtime purchases."
        },
        {
            icon: ShieldCheck,
            title: "Reliability",
            description: "Our platform ensures secure, seamless, and error-free transactions, so you can trust us for fast and dependable service every time."
        },
        {
            icon: CurrencyUsd,
            title: "Affordability",
            description: "We offer highly competitive prices, discounts, and bonuses to give you the best value for your money when purchasing data and airtime."
        },
        {
            icon: Headset,
            title: "24/7 Support",
            description: "Our dedicated customer service team is available round the clock to assist with any inquiries, complaints, or transaction issues."
        },
        {
            icon: AccountCircle,
            title: "User-Friendly Experience",
            description: "Our website is designed for smooth navigation, making it easy for users of all levels to buy data and airtime without hassle."
        },
        {
            icon: Flash,
            title: "Instant Delivery",
            description: "We guarantee quick and automatic top-ups, ensuring that your data and airtime are credited immediately after payment."
        }
    ];
</script>

<div class="mt-10 flex justify-center">
    <div class="grid grid-cols-[350px] gap-5 @3xl:grid-cols-[350px_350px]  @5xl:grid-cols-[350px_350px_350px]">
        {#each services as {icon, title, description}}
            <div class="text-center flex flex-col items-center p-2 py-5 shadow-sm shadow-gray-600 rounded-xl">
                <svelte:component this={icon} class="text-gold text-2xl" />
                <p class="font-bold  text-xl text-purple">{title}</p>
                <Small text = {description} />
            </div>
        {/each}
    </div>
</div>