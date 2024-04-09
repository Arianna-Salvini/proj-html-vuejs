<script>
import ButtonText from "./ButtonText.vue";
import ButtonPlay from "./ButtonPlay.vue";
import SectionTitle from "./SectionTitle.vue"

export default {
    name: 'AppMain',
    components: {
        ButtonText,
        ButtonPlay,
        SectionTitle,
    },
}
</script>

<template>
    <main>
        <section class="gaming_company d_flex">
            <div class="half_container element d_flex">
                <div class="image_box">
                    <img class="experience_img" src="../../public/img/exprince.jpg" alt="">
                    <img class="experience_shape" src="../../public/img/exprience-shape.png"
                        alt="public/img/exprience-shape.png">
                </div>
            </div>
            <!-- /.conteiner_element -->
            <div class="half_container d_flex">
                <div class="text_box">
                    <div class="title_section">
                        <SectionTitle title="we are the best game company" titleSection="12 Year Experience" />
                    </div>

                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque aperiam aspernatur corporis illo
                        cupiditate commodi, architecto sequi provident pariatur temporibus sapiente sit praesentium iste
                        voluptate et odit vero dicta nihil harum, consequuntur molestiae dolore! Ut veritatis laudantium
                        ab
                        esse fuga.</p>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusantium minus nihil, nostrum animi
                        commodi quae.</p>
                    <ul class="list_check">
                        <li>
                            <i class="fa-regular fa-circle-check green"></i>
                            Accusantium minus nihil
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check green"></i>
                            Neque aperiam aspernatur corporis
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check green"></i>
                            Neque aperiam aspernatur corporis
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check green"></i>
                            Neque aperiam aspernatur corporis
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check green"></i>
                            Neque aperiam aspernatur corporis
                        </li>
                    </ul>

                    <div class="button_area d_flex">
                        <ButtonText title="Discover More" iconButton="fa-solid fa-right-long" />
                        <ButtonPlay />
                    </div>
                </div>

            </div>
            <!-- /.container_text -->
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
        <section class="latest_news">

        </section>
        <!-- /.latest_news -->
    </main>
</template>

<style>
main {
    section {
        width: 100%;
        background-size: cover;
        background-position: center;
    }

    .overlay {
        background-color: var(--rax-darker);
        background-blend-mode: overlay;
    }

    .green {
        color: var(--rax-secondary);
    }

    /*  */
    .half_container.element {
        justify-content: flex-end;
    }

    .half_container {
        width: 50%;
        height: 100%;
        padding: 2.5rem;
        color: var(--rax-light);
        /* border: 1px solid white; */

        /* left half of section */
        .image_box {
            width: 577px;
            height: 567px;
            padding: 4.4rem;
            background-image: url(public/img/shape1.png), url(public/img/shape2.png);
            background-size: 438px, 254px;
            background-repeat: no-repeat;
            background-position: left top, right bottom;
            position: relative;

            .experience_img {
                width: 490px;
                position: absolute;
                top: 40px;
                left: 40px;
            }

            .experience_shape {
                width: 115px;
                height: 115px;
                position: absolute;
                top: 40px;
                left: -85px;
            }

        }
    }

    /* right half of section */

    .text_box {
        width: 640px;
        font-size: 1rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;

        &>* {
            padding-bottom: 2.5rem;
        }

        .list_check {
            list-style-type: none;
        }

        & ul {
            padding-bottom: 1rem;
        }

        & li {
            padding-bottom: 1.5rem;
        }

        &>p {
            line-height: 1.7rem;
            font-weight: 100;
            word-spacing: 0.2rem;
        }


    }



}

.gaming_company {
    height: 1016px;
    background-color: var(--rax-darkest);
    padding-top: 12.5rem;
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
    background-image: url(public/img/test-group.png), url(public/img/test-grouptwo.png);
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
</style>
