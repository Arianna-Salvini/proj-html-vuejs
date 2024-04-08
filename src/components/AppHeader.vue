<script>
import NavigationBar from "./NavigationBar.vue";
import ButtonText from "./ButtonText.vue"

export default {
    name: 'AppHeader',
    components: {
        NavigationBar,
        ButtonText,
    }
}
</script>

<template>
    <header>
        <div class="container">
            <NavigationBar />
            <div class="hero d_flex">
                <div>
                    <h4 id="welcome">Welcome to raxg</h4>
                    <h2>Are youready for your next challenge?</h2>
                    <ButtonText title="Read More" iconButton="fa-solid fa-right-long" />
                </div>
            </div>
        </div>

    </header>
</template>

<style>
header {
    background-image: url(public/img/banner1.png);
    width: 100%;
    height: 900px;
    color: var(--rax-light);
}

.hero {
    text-align: center;
    justify-content: center;
    height: 700px;
    text-transform: uppercase;

    #welcome {
        color: var(--rax-secondary);
        font-size: 1rem;
    }

    & h2 {
        font-size: 4rem;
    }
}
</style>
