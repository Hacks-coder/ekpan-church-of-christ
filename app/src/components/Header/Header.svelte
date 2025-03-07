<script>
    import IconMenu from '~icons/mdi/menu'
    
    const navigationLinks = [
        {href: "/home", child: "Home"},
        {href: "about", child: "About"},
        {href: "customer-care", child: "Contact"},
        {href: "sermons", child: "Sermons"}
    ]
    let isNavigationOpen = false;
    const toggleNavigation = () => {
        isNavigationOpen = !isNavigationOpen;
    }
</script>


<header class="@container font-main font-bold">
    <div class="@3xl:flex @3xl:justify-evenly @3xl:gap-5 @3xl:p-5">
        <nav class="flex justify-between">
        <p class="text-2xl font-title font-bold">Ekpan</p>
        <IconMenu class="text-3xl text-gold @3xl:hidden" onclick={toggleNavigation}/>
        </nav>
        {#if isNavigationOpen}
        <div class="flex justify-end @3xl:hidden">
            <div class="flex flex-col gap-0">
                {#each navigationLinks as {href, child}}
                    <a {href} onclick={toggleNavigation}>{child}</a>
                {/each}
            </div>
        </div>
        {/if}
        <div class="hidden @3xl:flex @3xl:gap-15">
            {#each navigationLinks as {href, child}}
                <a {href} onclick={toggleNavigation}>{child}</a>
            {/each}
        </div>
        <div class="hidden @3xl:flex @3xl:gap-5">
            <a href="/login" class="text-blue mt-2">Login</a>
            <a href="/register" class="bg-blue px-7 py-2 rounded-full text-white font-bold">Register</a>
        </div>
    </div>
</header>