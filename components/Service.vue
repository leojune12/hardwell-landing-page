<template>
    <div class="pt-5">
        <div class="container-xxl py-5">
            <div class="primary-text text-4xl text-md-5xl text-lg-6xl mb-4">
                Explore Service
            </div>
            <div class="secondary-text text-base text-md-xl mb-5 mx-auto">
                The sky was cloudless and of a deep dark blue spectacle before us was indeed sublime.
            </div>
            <div class="row services g-5 pt-0 pt-md-5">
                <div class="col-md-4">
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
                <div class="col-md-4">
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
                <div class="col-md-4">
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
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
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
</style>