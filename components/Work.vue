<template>
    <div class="work-section">
        <div class="container-xxl py-5 header">
            <div class="primary-text text-4xl text-md-5xl text-lg-6xl mb-4">
                Discover Our Work
            </div>
            <div class="secondary-text text-base text-md-xl mx-auto">
                Web designer is responsible for creating the design and layout of a website.
            </div>
        </div>
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
</template>
<script>
export default {
    
}
</script>
<style lang="scss">
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
    }
</style>