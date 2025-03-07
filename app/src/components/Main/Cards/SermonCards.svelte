<script>

	import Gray from "../Texts/Gray.svelte";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
    const sermons = [
    {
        timeOfReading: "10 Mins. Read",
        sermonPhoto: "/sermon/img1.png",
        dateOfPublish: "30 Jan. 2025",
        sermonTopic: "The Truth About the Law of Tithing",
        description: "The Bible discusses the law of tithe extensively in both the Old and New Testaments, shedding light on its significance in our lives."
    },
    {
        timeOfReading: "12 Mins. Read",
        sermonPhoto: "/sermon/img2.jpg",
        dateOfPublish: "05 Feb. 2025",
        sermonTopic: "Faith in the Midst of Uncertainty",
        description: "A deep dive into how faith can be a guiding light during uncertain times, supported by modern testimonies and scriptural insights."
    },
    {
        timeOfReading: "8 Mins. Read",
        sermonPhoto: "/sermon/img3.jpg",
        dateOfPublish: "12 Feb. 2025",
        sermonTopic: "Embracing Grace and Forgiveness",
        description: "Exploring the transformative power of God's grace and the healing benefits of forgiveness in everyday life."
    },
    {
        timeOfReading: "15 Mins. Read",
        sermonPhoto: "/sermon/img4.jpg",
        dateOfPublish: "20 Feb. 2025",
        sermonTopic: "Walking in the Spirit",
        description: "A guide to living a life enriched by the Holy Spirit, highlighting practical steps to cultivate spiritual growth."
    },
    {
        timeOfReading: "9 Mins. Read",
        sermonPhoto: "/sermon/img5.jpg",
        dateOfPublish: "28 Feb. 2025",
        sermonTopic: "The Power of Community and Fellowship",
        description: "An engaging look at how community and fellowship not only foster unity but also nurture individual spiritual journeys."
    },
    {
        timeOfReading: "11 Mins. Read",
        sermonPhoto: "/sermon/img6.jpg",
        dateOfPublish: "10 Mar. 2025",
        sermonTopic: "Hope in Times of Darkness",
        description: "A message of hope and resilience, reminding us that even in the darkest moments, God's light continues to shine."
    }
    ];


</script>



<div>
    <div class="w-80 shadow-xs shadow-gray-500 rounded-2xl px-2 py-2">
        
    </div>
</div>


<div class="@container flex justify-center mt-20">
    <div class="grid grid-cols-[330px] gap-10 @xl:grid-cols-[300px_300px] @4xl:grid-cols-[250px_250px_250px] @6xl:grid-cols-[350px_350px_350px]">
        {#each sermons as {timeOfReading, sermonPhoto, sermonTopic, description, dateOfPublish}}
           <div class="shadow-sm shadow-gray rounded-2xl px-2 py-5">
                <div class="p-3 w-70 h-50 rounded-2xl bg-cover bg-center @4xl:w-60 @6xl:w-80" style={`background-image: url(${sermonPhoto})`}>
                    <div class="bg-gray px-10 rounded-full py-1 w-fit"><Small text = {timeOfReading} /></div>
                </div>
                <Gray text = {dateOfPublish} />
                <div>
                    <Title text = {sermonTopic} />
                    <Gray text = {description} />
                </div>
           </div>
        {/each}
    </div>
</div>