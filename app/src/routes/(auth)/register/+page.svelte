<script>


    import IconMail from '~icons/fa-solid/envelope'; 
    import IconLock from '~icons/mdi/lock';
	import Title from '../../../components/Main/Texts/Title.svelte';
	import Small from '../../../components/Main/Texts/Small.svelte';
</script>


<section>
        <div>
            <Title text = "Welcome back" />
            <Title text = "Registration System" />
            <Small text = "Fill out all the fields" />
            <form class="flex flex-col items-center gap-5 mt-5">
                <div class="flex items-center gap-2 border-r-10 border-blue w-80 h-13 bg-lowWhite px-3 @md:w-100 @md:h-15 @xl:w-80 @2xl:w-100 @2xl:h-15 @4xl:w-120">
                    <IconMail class="text-blue text-2xl" />
                    <input type="email" placeholder="Email" class="outline-none border-none bg-transparent flex-1 h-full text-lg">
                </div>
                <div class="flex items-center gap-2 border-r-10 border-blue w-80 h-13 bg-lowWhite px-3 @md:w-100 @md:h-15 @xl:w-80 @2xl:w-100 @2xl:h-15 @4xl:w-120">
                    <IconLock class="text-blue text-2xl" />
                    <input type="password" placeholder="Password" class="outline-none border-none bg-transparent flex-1 h-full text-lg">
                </div>
                <div class="flex gap-10 justify-between w-full">
                    <Small text = "I have an account" />
                    <a href="/login" class="text-blue">Login</a>
                </div>
                <button class="w-80 h-13 text-white font-bold bg-blue rounded-md @md:w-100 @xl:w-80 @2xl:w-100 @4xl:w-120">Register</button>
            </form>
        </div>
</section>