<script>
    import ProductCard from "./ProductCard.svelte";
    import SectionWrapper from "./SectionWrapper.svelte";
    let productFeatures = [
        {
            featureList: [
                "Provide comprehensive eye examinations",
                "Detect eye conditions early",
                "Ensure accurate prescription updates",
                "Assess overall eye health and vision quality",
            ],
            description:
                "We offer a full suite of eye tests to assess the quality of your vision.",
            imgUrl: "assets/eye-exam.jpg",
        },
        {
            featureList: [
                "Offer a wide selection of stylish frames",
                "Craft lenses with precise prescriptions",
                "Provide custom fit and comfort adjustments",
                "Selection of Frames From Your Favourite Brands",
            ],
            description:
                "Lenses that fit your needs and frames that fit your style.",
            imgUrl: "assets/glasses-with-slightly-rounded-frame.jpg",
        },
        {
            featureList: [
                "Supply a variety of contact lens options for all needs",
                "Ensure a comfortable and secure fit",
                "Offer daily, bi-weekly, and monthly lens options",
                "Provide expert guidance for first-time wearers",
            ],
            description:
                "Enter as much information about yourself as you desire to ensure all workouts are personalized to your every need.",
            imgUrl: "assets/contact-lens.jpeg",
        },
    ];
</script>

<SectionWrapper id="product">
    <div
        class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:pb-14"
    >
        <div class="flex flex-col gap-2">
            <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
                You can see what we offer below
            </p>
            <h3
                class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
            >
                Our Services
            </h3>
        </div>

        {#each productFeatures as productFeature, index}
            <ProductCard {productFeature} {index}>
                {#if index === 0}
                    Comprehensive Eye <span class="text-indigo-400 font-medium"
                        >Testing</span
                    >
                {:else if index === 1}
                    <span class="text-indigo-400 font-medium"> Frames </span> From
                    The Best Brands
                {:else}
                    Stealth With <span class="text-indigo-400 font-medium"
                        >Contact Lenses</span
                    >
                {/if}
            </ProductCard>
        {/each}
    </div>
</SectionWrapper>
