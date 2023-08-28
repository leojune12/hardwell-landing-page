<template>
    <div class="container-xxl py-5">
        <div class="row gy-5">
            <div class="col-md-6">
                <div class="d-flex position-relative justify-content-end img-section pe-0 pe-md-4 pe-lg-5 pb-0 pb-md-4 pb-lg-5">
                    <img src="/images/about.png" alt="" class="object-fit-lg-contain img-fluid mx-auto">
                    <div class="growth-card p-4 p-lg-5 position-absolute">
                        <div class="value d-flex align-items-end mb-3 text-6xl text-md-7xl">
                            68%
                            <div class="up-arrow-container d-flex align-items-center justify-content-center ms-3 mb-2">
                                <img src="/images/up-arrow.svg" width="24" height="24" alt="">
                            </div>
                        </div>
                        <div class="description text-xl text-md-2xl">
                            Extra growth for <br> your company.
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-md-6 text-center text-md-start pt-5">
                <div class="text-section mx-auto">
                    <div class="about-text text-center text-md-start mb-3">
                        About
                    </div>
                    <div class="primary-text text-4xl text-md-5xl text-lg-6xl mb-3">
                        Creating, Communicating <br> & Delivering
                    </div>
                    <div class="secondary-text mb-3">
                        Web designers plan, create and code internet sites and web pages, many of which combine text with sounds, pictures, graphics and video clips.
                    </div>
                    <div>
                        <a href="#" class="btn learn-more-btn px-3 px-md-0">
                            Learn More
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    @import "~/assets/scss/mixins/breakpoints";

    .img-section {

        .growth-card {
            border-radius: 5px;
            background: #EA3D3C;
            bottom: -32px;
            right: 0px;

            .value {
                color: var(--set-1-color-34, #FFF);
                /* Regular/70px */
                font-family: Inter;
                // font-size: 70px;
                font-style: normal;
                font-weight: 400;
                // line-height: 56px; /* 110% */
                letter-spacing: -2px;

                .up-arrow-container {
                    width: 38px;
                    height: 38px;
                    background: #FFFFFF;
                    border-radius: 100%;
                }
            }

            .description {
                color: var(--set-1-color-34, #FFF);
                /* Regular/24px */
                font-family: Inter;
                // font-size: 24px;
                font-style: normal;
                font-weight: 400;
                // line-height: 36px; /* 150% */
            }
        }
    }

    @include media-breakpoint-up(md) {
        .img-section {

            .growth-card {
                bottom: 0px;
                right: 0px;
            }
        }
    }

    .text-section {

        max-width: 500px;

        .about-text {
            color: rgba(51, 51, 51, 0.50);
            font-family: Epilogue;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 32px; /* 200% */
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        .primary-text {
            color: #333;
            font-family: Epilogue;
            // font-size: 56px;
            font-style: normal;
            font-weight: 700;
            // line-height: 64px; /* 114.286% */
        }

        .secondary-text {
            color: rgba(51, 51, 51, 0.50);
            font-family: Epilogue;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 32px; /* 200% */
        }

        .learn-more-btn {
            color: #333;
            font-family: Epilogue;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 32px; /* 200% */
        }
    }
</style>