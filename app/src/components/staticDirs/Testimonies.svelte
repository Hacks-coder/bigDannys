<script>
	import Aqua from "../Texts/Aqua.svelte";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";


    const testimonies = [
        { photo: "/testimonies/img1.jpg", person: "Oghenewire", testimony: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ullamcorper scelerisque mi, in malesuada felis malesuada vel." },
        { photo: "/testimonies/img2.jpg", person: "Amarachi Akie", testimony: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ullamcorper scelerisque mi, in malesuada felis malesuada vel." },
        { photo: "/testimonies/img3.jpg", person: "Kevwe Arias", testimony: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ullamcorper scelerisque mi, in malesuada felis malesuada vel." }
    ];
</script>

<style>
    @media (prefers-reduced-motion: no-preference) {
        .testimony-card {
            transform: translateY(70px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
            animation-range: entry 20% cover 50%;
        }

        @keyframes fade-in-up {
            to {
                transform: translateY(0);
            }
        }

        /* Hover effect */
        .testimony-card:hover {
            transform: scale(1.05);
            transition: transform 0.3s ease-in-out;
        }
    }
</style>

<section class="@container mt-30">
    <div class="text-center">
        <Aqua text="TESTIMONIALS" />
        <Title text="Read What Others Have To Say" />
    </div>
    <div class="flex flex-col gap-15 mt-20 items-center @2xl:flex-row @2xl:justify-center">
        {#each testimonies as item}
            <div class="testimony-card shadow-sm shadow-gray-500 relative bg-darkPurple mt-10 size-56 rounded-xl text-center pl-2 pr-2 @md:size-64">
                <div style={`background-image: url(${item.photo})`} class="absolute rounded-full bg-cover size-32 bg-base top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2 shadow-sm shadow-black border-4 border-white"></div> 
                <Small text={item.person} className="mt-20"/>  
                <p class="text-xs mt-2">{item.testimony}</p>     
            </div>
        {/each}
    </div>
</section>
