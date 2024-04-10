<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import SectionTitle from "../elements/SectionTitle.vue";


export default {
    name: 'TeamMembers',
    components: {
        ButtonNext,
        ButtonBack,
        SectionTitle,
    },
    data() {
        return {
            cards: [
                {
                    image: 'public/img/team1.png',
                    name: 'Cristiano Messi',
                    role: 'CEO/Founder',
                },
                {
                    image: 'public/img/team2.png',
                    name: 'Sergio Naymer',
                    role: 'Programmer',
                },
                {
                    image: 'public/img/team3.png',
                    name: 'Antonella Rocca',
                    role: 'Project Manager',
                },
                {
                    image: 'public/img/team4.png',
                    name: 'Lionel Ramos',
                    role: 'Game Designer',
                },
            ]
        }
    }
}
</script>

<template>
    <section class="team_member">
        <div class="container ">
            <div class="top_section d_flex">
                <div class="half_container">
                    <div class="titles">
                        <SectionTitle title="our experts team members" titleSection="Team Members" />
                    </div>
                </div>
                <div class="half_container .right">
                    <div class="button_box d_flex ">
                        <ButtonBack />
                        <ButtonNext />
                    </div>
                </div>
            </div>
            <div class="bottom_section  d_flex">
                <div v-for="(card, index) in cards" :key="index" class="tranding-games">
                    <div class="box_card_game">
                        <div class="box_img">
                            <img :src="card.image" alt="">
                        </div>
                        <div class="box_card_text d_flex">
                            <div class="description_game">
                                <h3>{{ card.name }}</h3>
                                <p>{{ card.role }}</p>
                            </div>
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
.team_member {
    height: 831px;
    background-color: var(--rax-darkest);
}


/* Style */

.half_container {
    width: 50%;
    height: 100%;
    padding: 7rem 0 0;

    .button_box {
        justify-content: flex-end;
    }

    .bottom_section {
        width: 300px;
        height: 400px;

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
}

.box_card_game:hover box_card_text {
    background-color: var(--rax-secondary);
    color: var(--rax-darkest);
}
</style>
