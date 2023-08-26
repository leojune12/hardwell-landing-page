<template>
    <div class="hero-section position-relative">
        <img src="/images/dots.svg" alt="" class="dots-left-1 d-none d-md-block">
        <img src="/images/dots.svg" alt="" class="dots-left-2 d-none d-md-block">
        <img src="/images/dots.svg" alt="" class="dots-right-1 d-none d-md-block">
        <img src="/images/dots.svg" alt="" class="dots-right-2 d-none d-md-block">
        <div class="container-xxl pt-5 pb-5 pb-md-0 d-flex flex-column flex-md-row align-items-center">
            <div class="hero-text">
                <div class="agency-name d-flex align-items-center text-md-2xl text-xl justify-content-md-start justify-content-center">
                    <div class="red-line me-1"></div>
                    Ninad Creative Agency
                </div>
                <div class="primary-text mb-3 text-4xl text-md-5xl text-lg-7xl text-center text-md-start position-relative">
                    Creative <span class="mind">Mind</span> With
                    Creative People <img src="/images/left-arrow.svg" alt="">
                </div>
                <div class="secondary-text mb-4 text-base text-md-lg text-center text-md-start">
                    It is a long established fact that a reader will be distracted by the readable content of a page when at its layout.
                </div>
                <div>
                    <button class="btn read-more-btn w-100 w-md-auto">
                        Read-More
                        <img src="/images/right-arrow.svg" alt="">
                    </button>
                </div>
            </div>
            <div class="d-flex position-relative hero-image ps-4 d-md-flex justify-content-center flex-grow-1 d-none">
                <img src="/images/stars.png" alt="" class="stars">
                <img src="/images/image-19.png" alt="" class="three-lines">
                <img src="/images/hero-main.png" alt="" class="main-image ps-5 object-fit-scale">
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
    .hero-section {
        background: #F2F2F2;
        .dots-left-1 {
            position: absolute;
            top: 48px;
            left: 0px;
            opacity: 0.2;
        }

        .dots-left-2 {
            position: absolute;
            top: 128px;
            left: 0px;
            opacity: 0.2;
        }

        .dots-right-1 {
            position: absolute;
            top: 452px;
            right: 0px;
            opacity: 0.2;
        }

        .dots-right-2 {
            position: absolute;
            top: 534px;
            right: 0px;
            opacity: 0.2;
        }

        .hero-text {
            @include media-breakpoint-up(md) {
                max-width: 700px;
            }

            .agency-name {
                color: #000;
                font-family: Open Sans;
                // font-size: 25px;
                font-style: normal;
                font-weight: 400;
                // line-height: normal;

                .red-line {
                    background: #EA3D3C;
                    width: 3px;
                    height: 20px;
                }
            }

            .primary-text {
                color: #0E1017;
                font-family: Open Sans;
                // font-size: 62px;
                font-style: normal;
                font-weight: 700;
                // line-height: 84px; /* 135.484% */

                .mind {
                    color: #EA3D3C;
                    font-family: Open Sans;
                    // font-size: 62px;
                    font-style: normal;
                    font-weight: 700;
                    // line-height: 84px;
                }

                img {
                    position: absolute;
                    width: 0px;
                    height: 0px;
                }

                @include media-breakpoint-up(md) {
                    img {
                        width: 80px;
                        height: 80px;
                        bottom: -36px;
                    }
                }

                @include media-breakpoint-up(lg) {
                    img {
                        width: 112px;
                        height: 112px;
                        bottom: -44px;
                    }
                }
            }

            .secondary-text {
                @include media-breakpoint-up(md) {
                    max-width: 600px;
                }

                color: #7B7D84;
                font-family: Inter;
                // font-size: 18px;
                font-style: normal;
                font-weight: 400;
                // line-height: 30px; /* 166.667% */
            }

            .read-more-btn {
                border-radius: 4px;
                background: #EA3D3C;

                color: #FFF;
                font-family: Poppins;
                font-size: 16px;
                font-style: normal;
                font-weight: 500;
                line-height: 26px; /* 162.5% */

                padding: 16px 32px;
            }
        }

        .hero-image {
            // .main-image {
            //     position: absolute;
            //     left: 84px;
            //     bottom: 0px;
            // }

            .stars {
                position: absolute;
                bottom: 32px;
                left: 0;
            }

            .three-lines {
                position: absolute;
                top: 144px;
                right: 74px;
            }
        }
    }
</style>