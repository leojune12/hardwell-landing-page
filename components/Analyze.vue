<template>
    <div class="container-xxl py-5">
        <div class="row gy-5">
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
        <div>
            <img src="/images/video-play.png" alt="">
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss">
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
</style>