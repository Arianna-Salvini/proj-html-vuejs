<script>
import GamingCompany from "./section/GamingCompany.vue";
import GamingArena from "./section/GamingArena.vue";
import LiveStreaming from "./section/LiveStreaming.vue";
import TrendingBattle from "./section/TrendingBattle.vue";
import TrendingGames from "./section/TrendingGames.vue";
import UpcomingMatch from "./section/UpcomingMatch.vue";
import TeamMembers from "./section/TeamMembers.vue";
import Testimonials from "./section/Testimonials.vue";
import GameShop from "./section/GameShop.vue";


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
        GameShop,
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

        <GameShop />
        <!-- /.gamer_shop -->
        <section class="latest_news">

        </section>
        <!-- /.latest_news -->
    </main>
</template>

<style>
/* Utility */

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







.latest_news {
    height: 977px;
    background-color: var(--rax-darkest);
}
</style>
