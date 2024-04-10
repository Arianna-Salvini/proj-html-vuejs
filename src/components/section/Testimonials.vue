<script>
import ButtonNext from "../elements/ButtonNext.vue";
import ButtonBack from "../elements/ButtonBack.vue";
import SectionTitle from "../elements/SectionTitle.vue";


export default {
    name: 'Testimonials',
    components: {
        ButtonNext,
        ButtonBack,
        SectionTitle,
    },
}
</script>

<template>
    <section class="testimonials">
        <div class="container ">
            <div class="top_section d_flex">
                <div class="half_container">
                    <div class="titles">
                        <SectionTitle title="What our client say" titleSection="Testimonials" />
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
.testimonials {
    height: 800px;
    /* double images? YES, ypu can!*/
    background-image: url(public/img/test-group.png), url(public/img/test-grouptwo.png);
    background-size: auto;
    background-repeat: no-repeat;
    background-position: top right, bottom left;
}

/* Style */

.half_container {
    width: 50%;
    height: 100%;
    padding: 7rem 0 0;
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
