<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import SectionTitle from "../elements/SectionTitle.vue";

export default {
    name: 'GameShop',
    components: {
        ButtonNext,
        ButtonBack,
        SectionTitle,
    },
}
</script>

<template>
    <section class="gamer_shop overlay">
        <div class="container ">
            <div class="top_section d_flex">
                <div class="half_container">
                    <div class="titles">
                        <SectionTitle title="Explore our shop" titleSection="Gamer Shop" />
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
.gamer_shop {
    height: 847px;
    background-image: url(public/img/shop-bg.png);
}

.overlay {
    background-color: var(--rax-darker);
    background-blend-mode: overlay;
}

/* Style */

.half_container {
    width: 50%;
    height: 100%;
    padding-top: 7rem;
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