<template>
    <div class="container-xxl py-5">
        <div class="primary-text text-center mb-5">
            Our Famous Clients
        </div>
        <div class="d-flex flex-column flex-md-row justify-content-center gap-5 gap-md-4 gap-lg-5">
            <div class="d-flex justify-content-center">
                <img src="/images/client-1.svg" alt="">
            </div>
            <div class="d-flex justify-content-center">
                <img src="/images/client-2.svg" alt="">
            </div>
            <div class="d-flex justify-content-center">
                <img src="/images/client-3.svg" alt="">
            </div>
            <div class="d-flex justify-content-center">
                <img src="/images/client-4.svg" alt="">
            </div>
            <div class="d-flex justify-content-center">
                <img src="/images/client-5.svg" alt="">
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
        font-size: 24px;
        font-style: normal;
        font-weight: 700;
        line-height: 32px; /* 133.333% */
    }

    .clients {
        display: inline-grid;
        grid-template-columns: auto auto auto auto auto;
        gap: 54px;
    }
</style>