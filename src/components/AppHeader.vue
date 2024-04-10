<script>
import NavigationBar from "./elements/NavigationBar.vue";
import ButtonText from "./elements/ButtonText.vue";
import ButtonPlay from "./elements/ButtonPlay.vue";

export default {
    name: 'AppHeader',
    components: {
        NavigationBar,
        ButtonText,
        ButtonPlay,
    },
    data() {
        return {
            menuVoices: [
                {
                    title: 'Home',
                    dropdownMenu: [
                        { subTitle: 'Home' },
                        { subTitle: 'Info' },
                        { subTitle: 'Contact' },
                        { subTitle: '404' },
                    ],

                },
                {
                    title: 'Pages',
                    dropdownMenu: [
                        { subTitle: 'Abaout Us' },
                        { subTitle: 'About Us' },
                        { subTitle: 'Matches' },
                        { subTitle: 'Team' },
                        { subTitle: 'Squad' },
                        { subTitle: 'Squad Details' },
                        { subTitle: 'Coming Soon' },
                        { subTitle: '404' },

                    ],

                },
                { titles: 'Tournament' },
                {
                    title: 'Shop',
                    dropdownMenu: [
                        { subTitle: 'Shop' },
                        { subTitle: 'Gamer Shop' },
                        { subTitle: 'Chart' },
                        { subTitle: 'Squad' },
                        { subTitle: '404' },
                    ],

                },
                {
                    title: 'Blog',
                    dropdownMenu: [
                        { subTitle: 'Blog' },
                        { subTitle: 'Latest News' },
                    ],

                },
                {
                    title: 'Contact',
                    dropdownMenu: ''
                },

            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <NavigationBar :menuVoices="menuVoices" />
            <div class="hero d_flex">
                <div>
                    <h4 id="welcome">Welcome to raxg</h4>
                    <h2>Are youready for your next challenge?</h2>
                    <div class="button_area d_flex">
                        <ButtonText title="Read More" iconButton="fa-solid fa-right-long" />
                        <ButtonPlay />
                    </div>
                    <!-- /.button_area -->

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

    .button_area {
        justify-content: center;
    }
}
</style>
