<script>
    import NameTag from "./NameTag.svelte";
</script>

<footer class="py-16 sm:py-20 md:py-24 px-4 md:px-8">
    <div
        class="max-w-[1200px] mx-auto w-full grid grid-cols-1 sm:grid-cols-2 md:grid-cols-5 gap-8 text-base"
    >
        <div class="flex flex-col gap-4 md:col-span-2">
            <NameTag />
            <p>©2024 Bhika Optometrist All rights reserved.</p>
        </div>
        <div class="flex flex-col gap-4">
            <p class="font-bold poppins text-base sm:text-lg">Support</p>
            <a
                href="tel:+27178191258"
                target="_blank"
                class="cursor-pointer hover:text-indigo-400 duration-200"
            >
                Contact Us <br />
                017 819 1258</a
            >
        </div>
        <div class="flex flex-col gap-4">
            <p class="font-bold poppins text-base sm:text-lg">Address</p>
            <a
                href="https://maps.app.goo.gl/F5fFwh9JqLvhF5KK9"
                target="_blank"
                class="cursor-pointer hover:text-indigo-400 duration-200"
            >
                Cnr of De Jager and, De Clercq St, Ermelo, 2351</a
            >
        </div>
        <div class="flex flex-col gap-4">
            <p class="font-bold poppins text-base sm:text-lg">Follow Us</p>
            <a
                href="https://www.instagram.com/bhika_optometrist/"
                target="_blank"
                class="cursor-pointer hover:text-indigo-400 duration-200"
            >
                <i class="fa-brands fa-instagram pr-2" />
                Instagram</a
            >

            <a
                href="https://web.facebook.com/Bhikaoptometrist/"
                target="_blank"
                class="cursor-pointer hover:text-indigo-400 duration-200"
            >
                <i class="fa-brands fa-facebook pr-2" />
                Facebook</a
            >
        </div>
    </div>
</footer>
