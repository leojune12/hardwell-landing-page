<template>
    <div class="container-xxl py-5">
        <div class="pt-5">
            <div class="primary-text text-4xl text-md-5xl text-lg-6xl mb-3 mb-md-4">
                Team Members
            </div>
            <div class="secondary-text text-base text-md-xl mx-auto">
                Combine text with sounds, pictures, graphics and video clips.
            </div>
        </div>
        <div class="team-members row gy-4 gy-md-0 py-5">
            <div class="col-md-6 col-lg-3 text-center">
                <div class="d-flex justify-content-center mb-4">
                    <img src="/images/team-1.png" alt="" class="img-fluid rounded-3">
                </div>
                <div class="name">
                    Bernarr Dominik
                </div>
                <div class="position">
                    Founder
                </div>
            </div>
            <div class="col-md-6 col-lg-3 text-center">
                <div class="d-flex justify-content-center mb-4">
                    <img src="/images/team-2.png" alt="" class="img-fluid rounded-3">
                </div>
                <div class="name">
                    Fabiana Capmany
                </div>
                <div class="position">
                    Account Manager
                </div>
            </div>
            <div class="col-md-6 col-lg-3 text-center">
                <div class="d-flex justify-content-center mb-4">
                    <img src="/images/team-3.png" alt="" class="img-fluid rounded-3">
                </div>
                <div class="name">
                    Alicia Stanger
                </div>
                <div class="position">
                    Designer
                </div>
            </div>
            <div class="col-md-6 col-lg-3 text-center">
                <div class="d-flex justify-content-center mb-4">
                    <img src="/images/team-4.png" alt="" class="img-fluid rounded-3">
                </div>
                <div class="name">
                    Anton Brownstein
                </div>
                <div class="position">
                    Developer
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
        max-width: 450px;
    }

    .team-members {
        .name {
            color: #333;
            font-family: Epilogue;
            font-size: 24px;
            font-style: normal;
            font-weight: 700;
            line-height: 32px; /* 133.333% */
        }
        .position {
            color: rgba(51, 51, 51, 0.50);
            font-family: Epilogue;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 32px; /* 200% */
        }
    }
</style>