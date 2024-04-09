<script>
import GamingCompany from "./section/GamingCompany.vue";
import GamingArena from "./section/GamingArena.vue";
import LiveStreaming from "./section/LiveStreaming.vue";
import TrendingBattle from "./section/TrendingBattle.vue";
import TrendingGames from "./section/TrendingGames.vue";
import UpcomingMatch from "./section/UpcomingMatch.vue";
import TeamMembers from "./section/TeamMembers.vue";
import Testimonials from "./section/Testimonials.vue";


export default {
    name: 'AppMain',
    components: {
        GamingCompany,
        GamingArena,
        LiveStreaming,
        TrendingBattle,
        TrendingGames,
        UpcomingMatch,
        TeamMembers,
        Testimonials,
    }
}
</script>

<template>
    <main>
        <GamingCompany />
        <!--/gaming_company Section -->

        <GamingArena />
        <!-- /.gaming_area -->

        <LiveStreaming />
        <!-- /.live_streaming -->

        <TrendingBattle />
        <!-- /.trending_battle -->

        <TrendingGames />
        <!-- /.trending_games -->

        <UpcomingMatch />
        <!-- /.upcoming_match -->

        <TeamMembers />
        <!-- /.team_member -->

        <Testimonials />
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
/* Utility */
.overlay {
    background-color: var(--rax-darker);
    background-blend-mode: overlay;
}

.green {
    color: var(--rax-secondary);
}

/* main {
    section {
        width: 100%;
        background-size: cover;
        background-position: center;
        color: var(--rax-light);
    }
} */

.trending_games {
    height: 816px;
    background-image: url(public/img/protfolio-vector.png);
}



.team_member {
    height: 831px;
    background-color: var(--rax-darkest);
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
