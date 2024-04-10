<script>
export default {
    name: 'AppFooter',

    data() {
        return {
            menuVoices: [
                { title: 'Home' },
                { title: 'Pages' },
                { title: 'Tournament' },
                { title: 'Shop' },
                { title: 'Blog' },
                { title: 'Contact' },

            ]
        }
    }
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="footer_container_top d_flex">

                <img src="../../public/img/menulogo.png" alt="">
                <ul class="menu_nav d_flex">
                    <li v-for="(menuVoice, index) in menuVoices" :key="index">
                        <a>{{ menuVoice.title }}</a>
                    </li>
                </ul>
            </div>
            <!-- /.footer_container_top -->
            <div class="footer_container_bottom d_flex">
                <div class="copirigh_text">
                    <span>Copiright © RaxG | </span>
                    <span>Designe by </span>
                    <span class="green">NextGenerationDev</span>
                </div>
                <div class="social_icon d_flex">
                    <div class="social_box d_flex">
                        <i class="fa-brands fa-facebook"></i>
                    </div>
                    <div class="social_box d_flex">
                        <i class="fa-brands fa-twitter"></i>
                    </div>
                    <div class="social_box d_flex">
                        <i class="fa-brands fa-linkedin-in"></i>
                    </div>
                    <div class="social_box d_flex">
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>

            </div>
            <!--footer_container_bottom -->
        </div>
    </footer>
</template>

<style>
footer {
    height: 370px;
    background-image: url(public/img/footer-bg.png);
    background-size: cover;
    background-position: center;
    background-color: var(--rax-darkest-overlay);
    background-blend-mode: overlay;
}

.footer_container_top {
    color: var(--rax-light);
    justify-content: space-between;
    padding: 10rem 0 2.5rem;
    border-bottom: 1px solid var(--rax-light);

    & li {
        list-style-type: none;
    }

    & a {
        text-decoration: none;
        padding: 1.5rem;
    }

}

.footer_container_bottom {
    color: var(--rax-light);
    justify-content: space-between;
    padding: 1.5rem 0;

    .social_box {
        width: 3rem;
        height: 3rem;
        margin: 0 0.5rem;
        background-color: var(--rax-darker);
        border-radius: 50%;
        color: var(--rax-light);
        justify-content: center;
    }

}

.social_box:hover {
    background-color: var(--rax-highlight);
}
</style>
