<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import SectionTitle from "../elements/SectionTitle.vue";

export default {
    name: 'LatestNews',
    components: {
        ButtonNext,
        ButtonBack,
        SectionTitle,
    },
}
</script>

<template>
    <section class="latest_news">
        <div class="container ">
            <div class="top_section d_flex">
                <div class="half_container">
                    <div class="titles">
                        <SectionTitle title="stay updated with our Latest News Articles" titleSection="Latest News" />
                    </div>
                </div>
                <div class="half_container .right">
                    <div class="button_box d_flex ">
                        <ButtonBack />
                        <ButtonNext />
                    </div>
                </div>
            </div>
            <!-- /.bottom_section -->
        </div>
    </section>
</template>

<style>
/* background */
.latest_news {
    height: 977px;
    background-color: var(--rax-darkest);
}

/* Style */

.half_container {
    width: 50%;
    height: 100%;
    padding: 7rem 0;
    text-align: center;

    .button_box {
        justify-content: flex-end;
    }

    .bottom_section {
        width: 300px;
        height: 390px;
    }
}
</style>