<script>


    import IconMail from '~icons/fa-solid/envelope'; 
    import IconLock from '~icons/mdi/lock';
	import Title from '../../../components/Main/Texts/Title.svelte';
	import Small from '../../../components/Main/Texts/Small.svelte';
</script>


<section>
        <div>
            <Title text = "Hello" />
            <Title text = "Contact Page" />
            <Small text = "What questions do you have for us today? Fill out all the field and we would respond shortly" />
            <form class="flex flex-col items-center gap-5 mt-5">
                <div class="flex items-center gap-2 border-r-10 border-blue w-80 h-13 bg-lowWhite px-3 @md:w-100 @md:h-15 @xl:w-80 @2xl:w-100 @2xl:h-15 @4xl:w-120">
                    <IconMail class="text-blue text-2xl" />
                    <input type="text" placeholder="Message Title:" class="outline-none border-none bg-transparent flex-1 h-full text-lg">
                </div>
                <div class="flex shadow-sm shadow-gray-300 items-center gap-2 border-r-10 border-blue w-80 h-50 bg-lowWhite px-3 @md:w-100 @md:h-15 @xl:w-80 @2xl:w-100 @2xl:h-15 @4xl:w-120">
                    <textarea placeholder="Ener message here..." class="outline-none border-none bg-transparent flex-1 h-50 text-lg"></textarea>
                </div>
                <button class="w-80 h-13 text-white font-bold bg-blue rounded-md @md:w-100 @xl:w-80 @2xl:w-100 @4xl:w-120">Send Message</button>
            </form>
        </div>
</section>