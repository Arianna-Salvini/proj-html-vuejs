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
        <section class="gaming_company">

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
        <sectio class="latest_news">

        </sectio>
        <!-- /.latest_news -->
    </main>
</template>

<style>
main {
    height: 627.5rem;

    section {
        width: 100%;
        background-size: cover;
        background-position: center;
    }

    .overlay {
        background-color: var(--rax-darker);
        background-blend-mode: overlay;
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
        background-image: url(public/img//test-group.png), url(public/img/test-grouptwo.png);
        background-size: auto;
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

}
</style>
