<script>
	import Fill from "../Buttons/Fill.svelte";
	import Gallery from "../Cards/Gallery.svelte";
	import DateCalander from "../StaticDirs/DateCalander.svelte";
	import Small from "../Texts/Small.svelte";


	import Title from "../Texts/Title.svelte";

</script>
<section class="@container mt-20 flex flex-col items-center px-5">
    <div class="border-2 border-black w-fit rounded-md px-5 py-3">I want to know Jesus</div>
    <div class="grid gap-10 @3xl:grid-cols-2 @3xl:gap-20">
        <div class="flex flex-col gap-2 ">
            <Title text = "Meet Our Members" />
            <Small text = 'We are committed to guiding you in deepening your relationship with God and worshiping Him authentically, as outlined in His Word. In John 4:24, Jesus teaches, "God is spirit, and those who worship him must worship in spirit and truth."' />
            <Small text = ' This means that true worship goes beyond rituals; it involves engaging sincerely with God through heartfelt devotion and aligning our lives with His truth.' />
            <div class="flex gap-2">
                <Fill text = "Join" />
                <DateCalander />
            </div>
        </div>
        <div>
            <Gallery />
        </div>
    </div>
</section>