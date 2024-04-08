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
    --rax-secondary: #05CC7C;
    --rax-highlight: #00AC4D;
    --rax-light: #ffffff;
    --rax-dark: #333287;
    --rax-darker: #202046;
    --rax-darkest: #191935;
    --rax-darkest-overlay: #19193580;
}

body {
    max-width: 1920px;
    background-color: var(--rax-darker);
}

.container {
    width: 70%;
    height: 100%;
    margin: auto;
    /* background-color: #05CC7C; */
}

.d_flex {
    display: flex;
    align-items: center;
}
</style>
