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
                        <SectionTitle title="What our clientas say" titleSection="Testimonials" />
                    </div>
                </div>
            </div>
            <!-- /.top_section -->
            <div class="bottom_container">
                <div class="bottom_box d_flex ">
                    <div class="testimonial_imag">
                        <img src="../../../public/img/test1.png" alt="">
                    </div>
                    <div class="testimonial_imag">
                        <img src="../../../public/img/test2.png" alt="">
                    </div>
                    <div class="testimonial_imag">
                        <img src="../../../public/img/test3.png" alt="">
                    </div>
                    <div class="testimonial_imag">
                        <img src="../../../public/img/test4.png" alt="">
                    </div>
                    <ButtonBack class="over back" />
                    <ButtonNext class="over next" />
                </div>
            </div>
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
}



.bottom_box {
    width: 300px;
    height: 390px;
    padding-top: 2rem;

}

.bottom_container {
    position: relative;
}

.over {
    position: absolute;
}

.over.next {
    right: 11%;
}
</style>
