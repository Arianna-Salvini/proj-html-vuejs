<script>
import NavigationBar from "./NavigationBar.vue";

export default {
    name: 'AppHeader',
    components: {
        NavigationBar,
    }
}
</script>

<template>
    <header>
        <div class="container">
            <NavigationBar />
        </div>
    </header>
</template>

<style>
header {
    background-image: url(public/img/banner1.png);
    width: 100%;
    height: 900px;
}
</style>
