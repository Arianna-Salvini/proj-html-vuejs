<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import ButtonPlay from "../elements/ButtonPlay.vue";
import SectionTitle from "../elements/SectionTitle.vue";

export default {
    name: 'TrendingGames',
    components: {
        ButtonNext,
        ButtonBack,
        ButtonPlay,
        SectionTitle,
    },
}
</script>

<template>
    <section class="trending_games">
        <div class="container ">
            <div class="top_section d_flex">
                <div class="half_container">
                    <div class="titles">
                        <SectionTitle title="Checkout our llive streaming" titleSection="Live Streaming" />
                    </div>
                </div>
                <div class="half_container .right">
                    <div class="button_box d_flex ">
                        <ButtonBack />
                        <ButtonNext />
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style>
/* background */
.trending_battle {
    height: 1988px;
    background-color: var(--rax-darkest);
}

/* Style */

.half_container {
    width: 50%;
    height: 100%;
    padding: 2.5rem;

    .button_box {
        justify-content: flex-end;
    }
}
</style>
