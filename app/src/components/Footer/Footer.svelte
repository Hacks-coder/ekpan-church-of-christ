<script lang="ts">


    const footerPath = [
        {
            title: "Main",
            text: [
                {title: "Home", href: "/home"},
                {title: "About", href: "/about"},
                {title: "Sermon", href: "/sermon"}         
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

<footer class="grid bg-darkBlue p-2 gap-10  mt-40 text-white grid-cols-1 md:grid-cols-2 md:place-items-center lg:grid-cols-3 lg:p-10">
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