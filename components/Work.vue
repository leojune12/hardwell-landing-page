<template>
    <div class="work-section py-0 py-md-5">
        <div class="container-xxl py-5 header">
            <div class="primary-text text-4xl text-md-5xl text-lg-6xl mb-4">
                Discover Our Work
            </div>
            <div class="secondary-text text-base text-md-xl mx-auto">
                Web designer is responsible for creating the design and layout of a website.
            </div>
        </div>
        <div class="pb-0 pb-md-5">
            <div class="content py-5">
                <div class="container-xxl">
                    <div class="row">
                        <div class="col-md-6 d-flex flex-column justify-content-center pb-5 pb-md-0 text-center text-md-start ps-md-5">
                            <div class="user-interface-text mb-3">
                                User Interface
                            </div>
                            <div class="primary-text text-3xl text-md-4xl mb-3 mx-auto m-md-0">
                                Creative Agency & Portfolio
                            </div>
                            <div class="secondary-text mx-auto m-md-0">
                                Web designers plan, create and code internet sites and web pages, text with sounds.
                            </div>
                        </div>
                        <div class="col-md-6 d-flex justify-content-center">
                            <img src="/images/image-12.png" alt="" class="mx-auto img-fluid">
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-xxl py-5">
            <swiper
                :slides-per-view="mediaBreakpointUp([
                    ['md', 2],
                ])"
                :modules="[Pagination]"
                :pagination="{
                    dynamicBullets: true,
                }"
                class="services pb-5 pb-md-0"
            >
                <swiper-slide>
                    <div class="d-flex justify-content-center">
                    <img src="/images/work-1.png" alt="" class="img-fluid">
                </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="d-flex justify-content-center">
                    <img src="/images/work-2.png" alt="" class="img-fluid">
                </div>
                </swiper-slide>
            </swiper>
            <div class="row categories gy-4 pt-5">
                <div class="col-md-4">
                    <div class="category-card p-5">
                        <div class="revenue-value">
                            4.200%
                        </div>
                        <div class="revenue-description">
                            Revenue
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="category-card p-5">
                        <div class="projects-value">
                            73+
                        </div>
                        <div class="projects-description">
                            Projects
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="category-card p-5">
                        <div class="uptime-value">
                            99.5+
                        </div>
                        <div class="uptime-description">
                            Uptime
                        </div>
                    </div>
                </div>
            </div>
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
    .work-section {
        .header {
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
                max-width: 500px;
            }
        }

        .content {
            background: #EA3D3C;

            .user-interface-text {
                color: #FFF;
                font-family: Epilogue;
                font-size: 16px;
                font-style: normal;
                font-weight: 400;
                line-height: 32px; /* 200% */
            }

            .primary-text {
                color: #FFF;
                font-family: Epilogue;
                // font-size: 40px;
                font-style: normal;
                font-weight: 700;
                // line-height: 48px; /* 120% */
                max-width: 500px;
            }

            .secondary-text {
                color: #FFF;
                font-family: Epilogue;
                font-size: 16px;
                font-style: normal;
                font-weight: 400;
                line-height: 32px; /* 200% */
                max-width: 500px;
            }
        }

        .categories {
            .category-card {
                border-radius: 8px;
                border: 1px solid #DDD;
                background: #FFF;
            }
            .revenue-value {
                color: #9CD161;
                text-align: center;
                font-family: Epilogue;
                font-size: 56px;
                font-style: normal;
                font-weight: 700;
                line-height: 64px; /* 114.286% */
            }
            .revenue-description {
                color: #9CD161;
                text-align: center;
                font-family: Epilogue;
                font-size: 20px;
                font-style: normal;
                font-weight: 400;
                line-height: 32px; /* 160% */
            }
            .projects-value {
                color: #F5AD0D;
                text-align: center;
                font-family: Epilogue;
                font-size: 56px;
                font-style: normal;
                font-weight: 700;
                line-height: 64px; /* 114.286% */
            }
            .projects-description {
                color: #F5AD0D;
                text-align: center;
                font-family: Epilogue;
                font-size: 20px;
                font-style: normal;
                font-weight: 400;
                line-height: 32px; /* 160% */
            }
            .uptime-value {
                color: #FB690C;
                text-align: center;
                font-family: Epilogue;
                font-size: 56px;
                font-style: normal;
                font-weight: 700;
                line-height: 64px; /* 114.286% */
            }
            .uptime-description {
                color: #FB690C;
                text-align: center;
                font-family: Epilogue;
                font-size: 20px;
                font-style: normal;
                font-weight: 400;
                line-height: 32px; /* 160% */
            }
        }
    }
</style>