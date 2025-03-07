<script>
	import Fill from "../Buttons/Fill.svelte";
	import Worship from "../Invitations/Worship.svelte";


	import Small from "../Texts/Small.svelte";
	import DateCalander from "./DateCalander.svelte";

</script>




<section class="@container mt-20 flex justify-center">
    <div class="grid gap-10 @3xl:grid-cols-2">
        <div class="px-5 flex flex-col gap-3 @3xl:mt-20">
            <p class="text-3xl font-title bg-gradient-to-r from-[#FD7747] to-[#0C2BD7] bg-clip-text text-transparent @md:text-4xl @3xl:text-5xl @5xl:text-7xl">WELCOME TO THE CHURCH OF CHRIST EKPAN</p>
            <Small text = "Let us help you know God better and how to worship effectively in spirit and in truth as written in HIs world" />
            <div class="flex gap-2">
                <Fill text = "Join" />
                <DateCalander />
            </div>
        </div>
        <div>
            <img src="/others/hero.png" alt="the hero section">
        </div>
    </div>
</section>