<script>
    import CtAs from "./CTAs.svelte";
    import Header from "./Header.svelte";
    import SectionWrapper from "./SectionWrapper.svelte";
    import Stars from "./Stars.svelte";
</script>

<SectionWrapper>
    <Header />
    <div
        class="flex flex-col gap-10 flex-1 items-center justify-center py-10 md:pb-14"
    >
        <div>
            <img src="assets/front-desk.png" alt="" />
        </div>
        <h2
            class="text-5xl sm:text-6xl md:text-7xl lg:text-8xl max-w-[1200px] mx-auto w-full text-center font-semibold"
        >
            <span class="text-indigo-400"> Experience</span> Life Through A
            <span class="text-slate-600">Sharper </span><span
                class="text-indigo-400"
            >
                Lens</span
            >
        </h2>
        <p
            class="text-xl sm:text-2xl md:text-3xl text-center max-w-[1000px] mx-auto w-full"
        >
            Book an Eye Test or Find Your Next Favorite Frames with Us
        </p>
        <p>
            <CtAs />
            <Stars />
        </p>
    </div>
</SectionWrapper>
