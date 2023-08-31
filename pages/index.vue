<template>
    <div>
        <NavBar />
        <Hero />
        <Service :breakpoint="breakpoint" />
        <About />
        <Work />
        <Analyze />
        <Team />
        <Testimonials />
        <Clients />
        <Blog />
        <Footer />
    </div>
</template>
<script setup>
    import { computed, onMounted, onUnmounted, ref } from "vue"

    function breakpoints() {
        let windowWidth = ref(window.innerWidth)

        const onWidthChange = () => windowWidth.value = window.innerWidth
        onMounted(() => window.addEventListener('resize', onWidthChange))
        onUnmounted(() => window.removeEventListener('resize', onWidthChange))

        const type = computed(() => {

            if (windowWidth.value >= 1400) return 'xxl'
            if (windowWidth.value >= 1200) return 'xl'
            if (windowWidth.value >= 992) return 'lg'
            if (windowWidth.value >= 768) return 'md'
            if (windowWidth.value >= 576) return 'sm'
            if (windowWidth.value >= 0) return 'xs'
        })

        const width = computed(() => windowWidth.value)

        return { width, type }
    }

    let { width, type } = breakpoints()

    const breakpoint = computed(() => width.value >= 768 ? 3 : 1)
</script>
<style lang="scss">
    body {
        overflow-y: auto !important;
    }
</style>