<template>
    <div>
        <TheHeader @sidenavToggle="displaySidenav = !displaySidenav" />
        <TheSidenav :show="displaySidenav" @close="displaySidenav = false" />
        <nuxt />
    </div>
</template>

<script>
import TheSidenav from '~/components/Navigation/TheSidenav.vue'
import TheHeader from '~/components/Navigation/TheHeader.vue'

export default {
    components: {
        TheSidenav,
        TheHeader,
    },
    data() {
        return {
            displaySidenav: false,
        }
    },
}
</script>

<style>
html {
    font-family: 'Open Sans', 'sans-serif';
}
body {
    margin: 0;
}
</style>
