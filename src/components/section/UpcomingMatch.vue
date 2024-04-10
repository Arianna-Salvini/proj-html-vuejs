<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import SectionTitle from "../elements/SectionTitle.vue";
import ButtonText from "../elements/ButtonText.vue"

export default {
    name: 'UpcomingMatch',
    components: {
        ButtonNext,
        ButtonBack,
        SectionTitle,
        ButtonText,
    },
    data() {
        return {
            cards: [
                {
                    image: 'public/img/m1.png',
                    gamerName: 'Ninja Warrior Gaming',
                    time: '9.45',
                    date: '1st November, 2022',
                },
                {
                    image: 'public/img/m2.png',
                    gamerName: 'Witch Gaming',
                    time: '9.45',
                    date: '1st November, 2022',
                },
                {
                    image: 'public/img/m3.png',
                    gamerName: 'SkullG Gaming',
                    time: '9.45',
                    date: '1st November, 2022',
                },
            ]
        }
    }
}
</script>

<template>
    <section class="upcoming_match overlay">
        <div class="container ">
            <div class="top_section d_flex">
                <div class="half_container">
                    <div class="titles">
                        <SectionTitle title="Keep eyes & Manage upcoming Battle" titleSection="Upcoming Match" />
                    </div>
                </div>
                <div class="half_container .right">
                    <div class="button_box d_flex ">
                        <ButtonBack />
                        <ButtonNext />
                    </div>
                </div>
            </div>

            <!-- TO FINISH -->

            <!-- <div class="bottom_section d_flex">
                <div v-for="(card, index) in cards" :key="index" class="match_cards">
                    <div class="img_team">
                        <img :src="card.image" alt="">
                    </div>
                    <div class="text_box_gamer">
                        <h3>{{ card.gamerName }}</h3>
                        <div class="button_generic_section d_flex">
                            <button class="icon_btn ">
                                <i class="fa-brands fa-youtube"></i>
                            </button>
                            <button class="icon_btn">
                                <i class="fa-solid fa-message"></i>
                            </button>
                        </div>
                        <div class="text_box_card">
                            <h3 class="hours">{{ card.time }}</h3>
                            <div class="date">{{ card.date }}</div>
                        </div>
                        <ButtonText title="View More" />
                    </div>
                </div> -->

        </div>
        <!-- /.bottom_section -->
        </div>
    </section>
</template>

<style>
/* background */
.upcoming_match {
    height: 1123px;
    background-image: url(public/img/v-bg.png);
}

/* Style title top section*/
.half_container {
    width: 50%;
    height: 100%;
    padding: 2.5rem;


    /* Next and Back Button */
    .button_box {
        justify-content: flex-end;
    }
}

/* Cards Style */
.match_cards {
    width: 420px;
    height: 690px;
    background-color: var(--rax-darker);
    padding: 1rem;
    border-radius: 10px;
    margin: 0.5rem;


    .img_team {
        width: 350px;
        height: 300px;
        border-radius: 10px;
        object-fit: cover;
    }

    .text_box_gamer {
        text-align: center;
    }
}

/* Buttons style */
.icon_btn {
    width: 3rem;
    aspect-ratio: 1;
    color: var(--rax-darkest);
    background-color: var(--rax-highlight);
    border-radius: 50%;
    border: none;
    margin: 0 0.4rem;


    & i {
        font-size: 1rem;
    }

    .battle_card:hover .icon_btn {
        background-color: var(--rax-darker);
        color: var(--rax-light);
        border: none;
    }
}
</style>
