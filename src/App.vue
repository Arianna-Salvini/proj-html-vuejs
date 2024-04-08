<script>

import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
    name: 'App',
    components: {
        AppHeader,
        AppMain,
        AppFooter,
    }
}


</script>

<template>
    <div>

        <AppHeader />

        <AppMain />

        <AppFooter />

    </div>
</template>

<style>
:root {
    --rax-primary: #4350FF;
    -rax-secondary: #05CC7C;
    --rax-highlight: #00AC4D;
    --rax-light: #ffffff;
    --rax-dark: #333287;
    --rax-darker: #202046;
    --rax-darkest: #191935;
}
</style>
