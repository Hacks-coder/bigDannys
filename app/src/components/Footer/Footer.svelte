<script lang="ts">
	import Title from "../Texts/Title.svelte";


    const footerPath = [
        {
            title: "Resources",
            text: [
                {title: "Airtime", href: "/"},
                {title: "Data", href: "/"},
                {title: "More", href: "/"}         
            ]
        },
        {
            title: "Media",
            text: [
                {title: "Facebook", href: "/"},
                {title: "Whatsapp", href: "/"},
                {title: "mail", href: "/"},
                {title: "Youtube", href: "/"}
            ]
        },
        {
            title: "Information",
            text: [
                {title: "blog", href: "/"},
                {title: "Private Policies", href: "/"},
                {title: "Terms and conditions", href: "/"}         
            ]
        },
    ]
</script>

<footer class="grid bg-white gap-10 p-5 mt-40 text-black grid-cols-1 md:grid-cols-2 md:place-items-center lg:grid-cols-3">
     {#each footerPath as {title, text}}
        <div>      
            <p class="text-purple font-bold font-title text-xl">{title}</p>
            {#each text as {title, href}}
                <div>
                    <a {href}>{title}</a>
                </div>  
            {/each}       
        </div>
    {/each}
</footer>