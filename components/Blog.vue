<template>
    <div class="container-xxl py-5">
        <div class="primary-text text-4xl text-md-5xl text-center">
            Latest From Blog
        </div>
        <swiper
            :slides-per-view="mediaBreakpointUp([
                ['md', 2],
                ['lg', 3],
            ])"
            :space-between="40"
            :modules="[Pagination]"
            :pagination="{dynamicBullets: true,}"
            class="blogs py-5 pb-lg-0"
        >
            <swiper-slide>
                <div class="item overflow-hidden mx-auto position-relative">
                    <div>
                        <img src="/images/blog-1.png" alt="" class="w-100">
                    </div>
                    <div class="p-4">
                        <div class="title">
                            Build prototypes with thousands of components.
                        </div>
                        <div class="description">
                            Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches.
                        </div>
                        <div>
                            <a href="#" class="stretched-link link-1">
                                Read more
                            </a>
                        </div>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide>
                <div class="item overflow-hidden mx-auto position-relative">
                    <div>
                        <img src="/images/blog-2.png" alt="" class="w-100">
                    </div>
                    <div class="p-4">
                        <div class="title">
                            Build prototypes with thousands of components.
                        </div>
                        <div class="description">
                            Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches.
                        </div>
                        <div>
                            <a href="#" class="stretched-link link-2">
                                Read more
                            </a>
                        </div>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide>
                <div class="item overflow-hidden mx-auto position-relative">
                    <div>
                        <img src="/images/blog-3.png" alt="" class="w-100">
                    </div>
                    <div class="p-4">
                        <div class="title">
                            Build prototypes with thousands of components.
                        </div>
                        <div class="description">
                            Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches.
                        </div>
                        <div>
                            <a href="#" class="stretched-link link-3">
                                Read more
                            </a>
                        </div>
                    </div>
                </div>
            </swiper-slide>
        </swiper>
    </div>
</template>
<script setup>
    // Import Swiper Vue.js components
    import { Swiper, SwiperSlide } from 'swiper/vue';
    
    // import required modules
    import { Pagination } from 'swiper/modules';

    // Import Swiper styles
    import 'swiper/css';
    import 'swiper/css/pagination';

    const props = defineProps({
        breakpoint: Object
    })

    let mediaBreakpointUp = (breakpoint) => {
        let slidesPerView = 1

        breakpoint.forEach(element => {
            if (props.breakpoint.width >= props.breakpoint.sizes[element[0]]) {
                slidesPerView = element[1]
            }
        })

        return slidesPerView
    }
</script>
<style lang="scss" scoped>
    .primary-text {
        color: #0D152E;
        font-family: Poppins;
        // font-size: 42px;
        font-style: normal;
        font-weight: 700;
        // line-height: normal;
        letter-spacing: -1.886px;
    }

    .blogs {
        .item {
            border-radius: 14px;
            border: 1px solid rgba(0, 0, 0, 0.12);
            max-width: 400px;

            &:hover {
                opacity: 0.9;
                background: #f1f1f1;
            }

            .title {
                color: #0D152E;
                font-family: Poppins;
                font-size: 20px;
                font-style: normal;
                font-weight: 700;
                line-height: 34px; /* 170% */
                letter-spacing: -0.66px;
            }

            .description {
                color: #81838C;
                font-family: Poppins;
                font-size: 16px;
                font-style: normal;
                font-weight: 400;
                line-height: 28px; /* 175% */
                letter-spacing: -0.5px;
            }

            a {
                font-family: Poppins;
                font-size: 16px;
                font-style: normal;
                font-weight: 700;
                line-height: normal;
                letter-spacing: -0.528px;
                text-decoration-line: underline;
            }

            .link-1 {
                color: #F5AD0D;
            }

            .link-2 {
                color: #AADF39;
            }

            .link-3 {
                color: #FB690C;
            }
        }
    }
</style>