<template>
    <div>
        <NavBar />
        <Hero />
        <Service :breakpoint="{
            sizes: sizes,
            width: width
        }" />
        <About />
        <Work :breakpoint="{
            sizes: sizes,
            width: width
        }" />
        <Analyze />
        <Team :breakpoint="{
            sizes: sizes,
            width: width
        }" />
        <Testimonials :breakpoint="{
            sizes: sizes,
            width: width
        }" />
        <Clients />
        <Blog :breakpoint="{
            sizes: sizes,
            width: width
        }" />
        <Footer />
    </div>
</template>
<script setup>
    import { computed, onMounted, onUnmounted, ref } from "vue"

    // Get current screen width
    let windowWidth = ref(window.innerWidth)
    const onWidthChange = () => windowWidth.value = window.innerWidth
    onMounted(() => window.addEventListener('resize', onWidthChange))
    onUnmounted(() => window.removeEventListener('resize', onWidthChange))
    const width = computed(() => windowWidth.value)

    let sizes = {
        xs: 0,
        sm: 576,
        md: 768,
        lg: 992,
        xl: 1200,
        xxl: 1400,
    }
</script>
<style lang="scss">
    body {
        overflow-y: auto !important;
    }

    .swiper-wrapper {
        padding: 0;
    }
</style>