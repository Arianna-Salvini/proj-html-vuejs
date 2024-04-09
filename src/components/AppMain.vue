<script>
import ButtonText from "./ButtonText.vue";
import ButtonPlay from "./ButtonPlay.vue";

export default {
    name: 'AppMain',
    components: {
        ButtonText,
        ButtonPlay,
    },
}
</script>

<template>
    <main>
        <section class="gaming_company d_flex">
            <div class="half_container element d_flex">
                <div class="image_box">
                    <img class="experience_img" src="../../public/img/exprince.jpg" alt="">
                    <img class="experience_shape" src="../..public/img/exprience-shape.png" alt="">
                </div>
            </div>
            <!-- /.conteiner_element -->
            <div class="half_container text"></div>
            <!-- /.container_text -->
        </section>
        <!--/gaming_company Section -->
        <section class="gaming_area">

        </section>
        <!-- /.gaming_area -->
        <section class="live_streaming overlay">

        </section>
        <!-- /.live_streaming -->
        <section class="trending_battle">

        </section>
        <!-- /.trending_battle -->

        <section class="trending_games">

        </section>
        <!-- /.trending_games -->
        <section class="upcoming_match overlay">

        </section>
        <!-- /.upcoming_match -->
        <section class="team_member">

        </section>
        <!-- /.team_member -->
        <section class="testimonials">

        </section>
        <!-- /.testimonials -->
        <section class="gamer_shop overlay">

        </section>
        <!-- /.gamer_shop -->
        <section class="latest_news">

        </section>
        <!-- /.latest_news -->
    </main>
</template>

<style>
main {
    section {
        width: 100%;
        background-size: cover;
        background-position: center;
    }

    .overlay {
        background-color: var(--rax-darker);
        background-blend-mode: overlay;
    }

    .half_container {
        width: 50%;
        height: 100%;
        padding: 2.5rem;
        border: 1px solid white;
        justify-content: flex-end;

        .image_box {
            width: 577px;
            height: 567px;
            background-image: url(public/img/shape1.png), url(public/img/shape2.png);
            background-size: 438px, 254px;
            background-repeat: no-repeat;
            background-position: left top, right bottom;
            position: relative;

            .experience_img {
                width: 490px;
                position: absolute;
                top: 40px;
                left: 40px;
            }

            .experience_shape {
                width: 115px;
                height: 115px;
                position: absolute;
                top: 40px;
                left: -74px;
            }
        }
    }

}

.gaming_company {
    height: 1016px;
    background-color: var(--rax-darkest);
}

.gaming_area {
    height: 802px;
    background-image: url(public/img/Vector.png);
}

.live_streaming {
    height: 834px;
    background-image: url(public/img/v-bg.png);
}

.trending_battle {
    height: 1988px;
    background-color: var(--rax-darkest);
}

.trending_games {
    height: 816px;
    background-image: url(public/img/protfolio-vector.png);
}

.upcoming_match {
    height: 1123px;
    background-image: url(public/img/v-bg.png);
}

.team_member {
    height: 831px;
    background-color: var(--rax-darkest);
}

.testimonials {
    height: 800px;
    /* double images? YES, ypu can!*/
    background-image: url(public/img/test-group.png), url(public/img/test-grouptwo.png);
    background-repeat: no-repeat;
    background-position: top right, bottom left;
}

.gamer_shop {
    height: 847px;
    background-image: url(public/img/shop-bg.png);
}

.latest_news {
    height: 977px;
    background-color: var(--rax-darkest);
}
</style>
