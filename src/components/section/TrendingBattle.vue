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
    data() {
        return {
            cards: [
                {
                    country1: 'Italy',
                    country2: 'India',
                    imgGamer1: 'public/img/t3.png',
                    imgGamer2: 'public/img/t4.png',
                    gamerName1: 'Ninja Gaming',
                    gamerName2: 'Witch Gaming',
                    gameName: 'PUBG Battleground',
                    descriptionGame: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde eaque soluta dicta laboriosam!',
                    time: '10.45',
                    date: '1st November, 2022',
                },
                {
                    country1: 'Italy',
                    country2: 'India',
                    imgGamer1: 'public/img/t1.png',
                    imgGamer2: 'public/img/t2.png',
                    gamerName1: 'King Gaming',
                    gamerName2: 'Witch Astro',
                    gameName: 'Assassain\'s Creed',
                    descriptionGame: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde eaque soluta dicta laboriosam!',
                    time: '9.45',
                    date: '1st November, 2022',
                },
                {
                    country1: 'Italy',
                    country2: 'India',
                    imgGamer1: 'public/img/t5.png',
                    imgGamer2: 'public/img/t6.png',
                    gamerName1: 'Dgn Gaming',
                    gamerName2: 'Joker Gaming',
                    gameName: 'Mortal Combat X',
                    descriptionGame: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde eaque soluta dicta laboriosam!',
                    time: '8.45',
                    date: '1st November, 2022',
                },
                {
                    country1: 'Italy',
                    country2: 'India',
                    imgGamer1: 'public/img/t7.png',
                    imgGamer2: 'public/img/t8.png',
                    gamerName1: 'Shark Gaming',
                    gamerName2: 'Krull Gaming',
                    gameName: 'Call of Deauty',
                    descriptionGame: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde eaque soluta dicta laboriosam!',
                    time: '4.45',
                    date: '1st November, 2022',
                },
            ]
        }
    }

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
            <div class="bottom box_battle_card ">
                <div v-for="(card, index) in cards" :key="index" class="battle_card d_flex">

                    <div class="gamer_card ">
                        <div class="img_box">
                            <img class="card_img" :src="card.imgGamer1" alt="">
                        </div>
                        <div class="card_battle_text">
                            <div class="country_gaming_arena"> {{ card.country1 }} </div>
                            <h3 class="gamer_name"> {{ card.gamerName1 }}</h3>
                        </div>
                    </div>

                    <div class="versus">
                        VS
                    </div>

                    <div class="gamer_card ">
                        <div class="img_box">
                            <img class="card_img" :src="card.imgGamer2" alt="">
                        </div>
                        <div class="card_battle_text">
                            <div class="country_gaming_arena"> {{ card.country2 }} </div>
                            <h3 class="gamer_name"> {{ card.gamerName2 }}</h3>
                        </div>
                    </div>

                    <div class="card_battle_description">
                        <h3>{{ card.gameName }}</h3>
                        <p>{{ card.descriptionGame }}</p>
                    </div>

                    <div class="battle_time d_flex">
                        <h3 class="hours">{{ card.time }}</h3>
                        <h4 class="date">{{ card.date }}</h4>
                        <div class="button_generic_section d_flex">
                            <button class="icon_btn ">
                                <i class="fa-brands fa-youtube"></i>
                            </button>
                            <button class="icon_btn">
                                <i class="fa-solid fa-message"></i>
                            </button>
                        </div>
                    </div>

                </div>

            </div>
            <!-- /.bottom box_battle_card -->
        </div>


    </section>
</template>

<style>
/* background */
.trending_battle {
    height: 1988px;
    background-color: var(--rax-darkest);
}

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

/* Battle cards */

.battle_card {
    height: 355px;
    background-color: var(--rax-darker);
    border: 1px solid var(--rax-secondary);
    padding: 2rem;
    margin: 2rem 0;
    border-radius: 10px;


    .gamer_card {
        width: 200px;
        height: 100%;

        .img_box {
            width: 100%;
            height: 70%;

            .card_img {
                width: 100%;
                height: 100%;
                background-color: var(--rax-darkest);
                padding: 1rem;
                border-radius: 10px 10px 0 0;
                object-fit: contain;
            }

        }

        .card_battle_text {
            background-color: var(--rax-dark);
            padding: 1rem;
            border-radius: 0 0 10px 10px;


            .country_gaming_arena {
                color: var(--rax-secondary);
                line-height: 2rem;
            }

            .gamer_name {
                font-size: 1.4rem;
            }
        }

    }

    .versus {
        color: var(--rax-secondary);
        background-color: var(--rax-darkest);
        font-size: 1.5rem;
        font-weight: 800;
        width: 8.5rem;
        aspect-ratio: 1;
        border-radius: 10px;
        margin: 1.5rem;
        text-align: center;
        line-height: 8.5rem;
    }

    .card_battle_description {
        margin: 3rem;
        width: 350px;

        >h3 {
            font-size: 2rem;
            padding-bottom: 1rem;
        }

        >p {
            font-weight: 100;
            line-height: 1.5rem;
            word-spacing: 3px;
        }
    }

    .battle_time {
        background-color: var(--rax-darkest);
        width: 190px;
        aspect-ratio: 1;
        border-radius: 10px;
        padding: 1rem;
        flex-direction: column;
        justify-content: center;

        .button_generic_section {
            justify-content: center;
            margin: 1rem;
        }

        .hours {
            font-size: 2rem;
            letter-spacing: 2px;
        }

        .date {
            font-size: 1rem;
            font-weight: 100;
            padding: 0.5rem 0;
        }
    }
}

/* Buttons style */
.icon_btn {
    width: 3rem;
    aspect-ratio: 1;
    color: var(--rax-darkest);
    background-color: var(--rax-secondary);
    border-radius: 50%;
    border: none;
    margin: 0 0.4rem;

    & i {
        font-size: 1rem;
    }

}

.icon_btn:hover {
    background-color: transparent;
    color: var(--rax-light);
}
</style>