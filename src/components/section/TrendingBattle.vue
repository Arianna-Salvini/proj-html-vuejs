<script>
import ButtonText from "../elements/ButtonText.vue";
import ButtonPlay from "../elements/ButtonPlay.vue";
import SectionTitle from "../elements/SectionTitle.vue";


export default {
    name: 'TrendingBattle',
    components: {
        ButtonText,
        ButtonPlay,
        SectionTitle,
    },
}
</script>

<template>
    <section class="trending_battle">
        <div class="container">
            <div class="top_menu">
                <SectionTitle title="Upcoming Match" titleSection="Trending Battle" />
                <ul class="menu_voices d_flex">
                    <li>
                        <a class="clicked" href="#">All</a>
                    </li>
                    <li>
                        <a href="#">Pludg</a>
                    </li>
                    <li>
                        <a href="#">COD</a>
                    </li>
                    <li>
                        <a href="#">AC</a>
                    </li>
                    <li>
                        <a class="last" href="#">MCX</a>
                    </li>
                </ul>
            </div>
            <div class="bottom box_battle_card">

            </div>
            <!-- /.bottom box_battle_card -->
        </div>
    </section>
</template>

<style>
/* Top menu section*/
.top_menu {
    padding-top: 8rem;
    display: flex;
    flex-direction: column;
    align-items: center;

    .menu_voices {
        list-style-type: none;
        padding-top: 3rem;

        .clicked {
            color: var(--rax-secondary);
            font-weight: 700;
        }

        .last {
            padding-right: 0;
        }
    }

    & a {
        font-size: 1.1rem;
        text-decoration: none;
        color: var(--rax-light);
        padding: 1rem 3rem 1rem 0;

    }
}
</style>

<!-- bottom section -->