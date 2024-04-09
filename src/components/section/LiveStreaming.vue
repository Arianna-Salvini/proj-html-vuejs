<script>
import ButtonBack from "../elements/ButtonBack.vue";
import ButtonNext from "../elements/ButtonNext.vue";
import SectionTitle from "../elements/SectionTitle.vue";
import ButtonPlay from "../elements/ButtonPlay.vue";

export default {
    name: 'LiveStreaming',
    components: {
        ButtonBack,
        ButtonNext,
        ButtonPlay,
        SectionTitle,
    },
    data() {
        return {
            slides: [
                { id: 1, image: 'public/img/v-small1.png', gameTitle: 'Call Of Deauty', gameDescription: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae, delectus!' },
                { id: 2, image: 'public/img/v-small2.png', gameTitle: 'Assaaain Creed', gameDescription: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae, delectus!' },
            ],
        }
    },
}
</script>

<template>
    <section class="live_streaming overlay">
        <div class="container d_flex ">
            <div class="half_container d_flex">
                <div class="carousel">
                    <img src="../../../public/img/v-1.png" alt="">
                    <div class="play_carousell">
                        <ButtonPlay class="play_btn_crsll" />
                        <h5>Call of Deauty</h5>
                    </div>
                </div>
            </div>
            <div class="half_container d_flex right">
                <div class="top d_flex">
                    <div class="titles">
                        <SectionTitle title="Checkout our llive streaming" titleSection="Live Streaming" />
                    </div>
                    <div class="button_box d_flex ">
                        <ButtonBack />
                        <ButtonNext class="button_next" />
                    </div>
                </div>
                <div class="bottom thumbnails d_flex">
                    <div class="thumbnail_box" v-for="(slide, index) in slides" :key="index">
                        <img :src="slide.image" alt="">
                        <h3 class="game_title">{{ slide.gameTitle }}</h3>
                        <p class="game_description">{{ slide.gameDescription }}</p>
                    </div>
                    <!-- /.button_box -->
                </div>
                <!-- /.bottom card_miniature -->
            </div>
        </div>
    </section>

</template>

<style>
/* background */
.live_streaming {
    height: 834px;
    background-image: url(public/img/v-bg.png);
}

/* Style */
.half_container {
    width: 50%;
    height: 100%;
    padding: 1rem;
    flex-direction: column;
    justify-content: center;

    .button_box {
        align-self: flex-end;
        justify-content: space-between;
    }

    .carousel {
        width: 100%;
        position: relative;

        >img {
            width: 100%;
        }

    }

    .thumbnails.bottom {
        justify-content: space-around;
        gap: 1rem;

        .thumbnail_box>img {
            width: 100%;
            margin-top: 2rem;
        }

        .thumbnail_box>h3 {
            padding: 1rem 0 0.7rem;
            color: var(--rax-light);
        }

        .thumbnails>p {
            font-weight: 100;
        }

    }

    .play_carousell {
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);

        .play_btn_crsll {
            width: 5rem;
            background-color: var(--rax-highlight);
        }

        >h5 {
            margin-top: 0.5rem;
        }
    }
}
</style>