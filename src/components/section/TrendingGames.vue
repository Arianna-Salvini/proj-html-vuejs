<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import SectionTitle from "../elements/SectionTitle.vue";

export default {
    name: 'TrendingGames',
    components: {
        ButtonNext,
        ButtonBack,
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
                        <SectionTitle title="choose who is the best in world!" titleSection="Trending Games" />
                    </div>
                </div>
                <div class="half_container .right">
                    <div class="button_box d_flex ">
                        <ButtonBack />
                        <ButtonNext />
                    </div>
                </div>
            </div>
            <div class="bottom_section">

            </div>
            <!-- /.bottom_section -->
        </div>
    </section>
</template>

<style>
/* background */

.trending_games {
    height: 816px;
    background-image: url(public/img/protfolio-vector.png);
}

/* Style */

.half_container {
    width: 50%;
    height: 100%;
    padding: 2.5rem;

    .button_box {
        justify-content: flex-end;
    }

    .bottom_section {
        width: 300px;
        height: 390px;
    }
}
</style>
