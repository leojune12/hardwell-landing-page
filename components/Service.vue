<template>
    <div class="pt-5">
        <div class="container-xxl py-5">
            <div class="primary-text text-4xl text-md-5xl text-lg-6xl mb-4">
                Explore Service
            </div>
            <div class="secondary-text text-base text-md-xl mb-5 mx-auto">
                The sky was cloudless and of a deep dark blue spectacle before us was indeed sublime.
            </div>
            <swiper
                :slides-per-view="mediaBreakpointUp([
                    ['md', 2],
                    ['lg', 3],
                ])"
                :modules="[Pagination]"
                :pagination="{dynamicBullets: true,}"
                class="services pb-5 pb-xl-0"
            >
                <swiper-slide>
                    <div class="item mx-auto">
                        <div class="mb-4 d-flex justify-content-center justify-content-md-start">
                            <img src="/images/athletics.png" alt="">
                        </div>
                        <div>
                            <div class="title text-center text-md-start">
                                Product Management
                            </div>
                            <div class="description text-center text-md-start">
                                Stay on top of your task lists and stay in touch with what's happening
                            </div>
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="item mx-auto">
                        <div class="mb-4 d-flex justify-content-center justify-content-md-start">
                            <img src="/images/archery-target.png" alt="">
                        </div>
                        <div>
                            <div class="title text-center text-md-start">
                                Design & Vreatives
                            </div>
                            <div class="description text-center text-md-start">
                                Stay on top of your task lists and stay in touch with what's happening
                            </div>
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="item mx-auto">
                        <div class="mb-4 d-flex justify-content-center justify-content-md-start">
                            <img src="/images/money-coins.png" alt="">
                        </div>
                        <div>
                            <div class="title text-center text-md-start">
                                Markething & Commuication
                            </div>
                            <div class="description text-center text-md-start">
                                Stay on top of your task lists and stay in touch with what's happening
                            </div>
                        </div>
                    </div>
                </swiper-slide>
            </swiper>
        </div>
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
        color: #333;
        text-align: center;
        font-family: Epilogue;
        // font-size: 56px;
        font-style: normal;
        font-weight: 700;
        // line-height: 64px; /* 114.286% */
    }

    .secondary-text {
        color: #333;
        text-align: center;
        font-family: Epilogue;
        // font-size: 20px;
        font-style: normal;
        font-weight: 400;
        // line-height: 32px; /* 160% */

        max-width: 550px;
    }

    .services {
        
        .item {
            max-width: 350px;

            .title {
                color: var(--set-01-color-03, #25373F);
                font-family: Epilogue;
                font-size: 22px;
                font-style: normal;
                font-weight: 600;
                line-height: 34px; /* 154.545% */
            }

            .description {
                color: var(--set-01-color-03, #25373F);
                /* Regular/16px */
                font-family: Inter;
                font-size: 16px;
                font-style: normal;
                font-weight: 400;
                line-height: 28px; /* 175% */
            }
        }
    }
</style>