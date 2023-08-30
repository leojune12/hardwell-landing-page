<template>
    <div class="py-5">
        <div class="container-xxl pb-5">
            <div class="row gy-5 gy-md-0 analyze-section">
                <div class="col-md-6 text-center text-md-start">
                    <div class="primary-text text-4xl text-md-5xl text-lg-6xl mb-4">
                        Analyze <br> & Improve
                    </div>
                    <div class="secondary-text mb-4 mx-auto mx-md-0">
                        Web designer is responsible for creating the design and layout of a website or web pages. It and can mean working on a brand new website.
                    </div>
                    <div>
                        <ul>
                            <li class="text-decoration-none mb-3">
                                <img src="/images/check.png" alt="">
                                Well Planned Architecture
                            </li>
                            <li class="text-decoration-none mb-3">
                                <img src="/images/check.png" alt="">
                                Accessible to All Users
                            </li>
                            <li class="text-decoration-none mb-3">
                                <img src="/images/check.png" alt="">
                                Mobile Compatibility
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-md-6 d-flex justify-content-center">
                    <img src="/images/analyze.png" alt="" class="img-fluid">
                </div>
            </div>
        </div>
        <div class="d-flex justify-content-center pt-5 video-section container-xxl">
            <iframe width="848" height="490" src="https://www.youtube.com/embed/noq-ZHTD2Cg" title="The Nuxt big thing in web development?" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        </div>
        <div class="row work-section mx-auto py-5 position-relative">
            <div class="bg-color"></div>
            <div class="container-xxl py-0 py-md-5">
                <div class="row text-center text-md-start">
                    <div class="col-md-6 primary-text mb-4 mb-md-0">
                        How We Work
                    </div>
                    <div class="col-md-6 secondary-text">
                        Web designers plan, create and code internet sites and web pages, many of which combine text with sounds, pictures, graphics and video clips.
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
    .analyze-section {
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
            max-width: 500px;
        }

        ul {
            padding: 0;

            li {
                list-style-type: none;
                color: #333;
                font-family: Epilogue;
                font-size: 16px;
                font-style: normal;
                font-weight: 400;
                line-height: 32px; /* 200% */
            }
        }
    }

    .video-section {
        position: relative;

        iframe {
            z-index: 100;
        }
    }

    .work-section {
        background: #F3F7F5;
        .container-xxl {
            max-width: 1000px;

            .primary-text {
                color: #000;
                font-family: Epilogue;
                font-size: 40px;
                font-style: normal;
                font-weight: 700;
                line-height: 48px; /* 120% */
            }

            .secondary-text {
                color: #000;
                font-family: Epilogue;
                font-size: 16px;
                font-style: normal;
                font-weight: 400;
                line-height: 32px; /* 200% */
            }
        }

        .bg-color {
            background: #F3F7F5;
            position: absolute;
            width: 100%;
            height: 245px;
            top: -245px;
            z-index: 50;
        }
    }
</style>