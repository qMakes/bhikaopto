<script>
    import { openModal } from "../store";
    import NameTag from "./NameTag.svelte";
</script>

<header class="flex flex-col relative z-20">
    <div
        class="max-w-[1400px] mx-auto w-full flex items-center justify-between p-4 py-6"
    >
        <a href="/">
            <NameTag />
        </a>
        <button
            on:click={() => ($openModal = true)}
            class="md:hidden grid place-items-center"
        >
            <i class="fa-solid fa-bars"></i>
        </button>
        <nav class="hidden md:flex items-center gap-4 lg:gap-6">
            <a
                href="#product"
                class="duration-200 hover:text-indigo-400 cursor-pointer"
                >Services</a
            >
            <a
                href="#reviews"
                class="duration-200 hover:text-indigo-400 cursor-pointer"
                >Reviews</a
            >
            <button class="specialBtn">
                <p>Book an appointment</p>
            </button>
        </nav>
    </div>
</header>
