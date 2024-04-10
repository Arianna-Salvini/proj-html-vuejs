<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import SectionTitle from "../elements/SectionTitle.vue";
import ButtonPlay from "../elements/ButtonPlay.vue";

export default {
    name: 'TrendingGames',
    components: {
        ButtonNext,
        ButtonBack,
        SectionTitle,
        ButtonPlay,
    },

    data() {
        return {
            cards: [
                {
                    image: 'public/img/protfolio1.png',
                    title: 'Assassin\'s Creed',
                    description: 'Donec sollicitudin malesuada.',
                },
                {
                    image: 'public/img/protfolio2.png',
                    title: 'Call Of deaury',
                    description: 'Donec sollicitudin malesuada.',
                },
                {
                    image: 'public/img/protfolio3.png',
                    title: 'Tomb Raider',
                    description: 'Donec sollicitudin malesuada.',
                },
                {
                    image: 'public/img/protfolio4.png',
                    title: 'Mortal Combat X',
                    description: 'Donec sollicitudin malesuada.',
                },
            ]
        }
    }
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
            <!-- / .top_section -->
            <div class="bottom_section d_flex">
                <div v-for="(card, index) in cards" :key="index" class="tranding-games">
                    <div class="box_card_game">
                        <div class="box_img">
                            <img :src="card.image" alt="">
                            <div class="badge">
                                New
                            </div>
                        </div>
                        <div class="box_card_text d_flex">
                            <div class="description_game">
                                <h3>{{ card.title }}</h3>
                                <p>{{ card.description }}</p>
                            </div>
                            <ButtonPlay />
                        </div>
                    </div>
                </div>
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
}

/* Card style */
.bottom_section {
    width: 300px;
    height: 380px;
    margin: 0rem 1.5rem;

    .tranding-games {
        width: 100%;
        height: 290px;
        margin: 1rem;

        .box_img {
            height: 100%;
            position: relative;
            overflow: hidden;
            object-fit: cover;
            object-position: center;

            .badge {
                position: absolute;
                top: 0;
                left: 0;
                padding: 0.5rem;
                background-color: var(--rax-secondary);
                color: var(--rax-light);
            }
        }

        .box_card_text {
            padding: 1rem;
            background-color: var(--rax-primary-dark);
            justify-content: space-between;

            .description_game>p {
                font-weight: 100;
                font-size: 1rem;
                padding-top: 5px;
            }

        }
    }
}
</style>
