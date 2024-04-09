<script>
import ButtonText from "../elements/ButtonText.vue";
import ButtonPlay from "../elements/ButtonPlay.vue";
import SectionTitle from "../elements/SectionTitle.vue";


export default {
    name: 'GamingCompany',
    components: {
        ButtonText,
        ButtonPlay,
        SectionTitle,
    },
}
</script>

<template>
    <section class="gaming_company d_flex">
        <div class="half_container right_to_center d_flex">
            <div class="image_box">
                <img class="experience_img" src="../../../public/img/exprince.jpg" alt="">
                <img class="experience_shape" src="../../../public/img/exprience-shape.png"
                    alt="public/img/exprience-shape.png">
            </div>
        </div>
        <!-- /.conteiner_element -->
        <div class="half_container d_flex">
            <div class="text_box">
                <!-- Component for titles -->
                <div class="title_section">
                    <SectionTitle title="we are the best game company" titleSection="12 Year Experience" />
                </div>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque aperiam aspernatur corporis illo
                    cupiditate commodi, architecto sequi provident pariatur temporibus sapiente sit praesentium iste
                    voluptate et odit vero dicta nihil harum, consequuntur molestiae dolore! Ut veritatis laudantium
                    ab
                    esse fuga.
                </p>
                <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusantium minus nihil, nostrum animi
                    commodi quae.
                </p>
                <!-- /description -->
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
                <!-- /Button area -->
            </div>

        </div>
        <!-- /.container_text -->
    </section>
</template>

<style>
/* // Background */
.gaming_company {
    height: 1016px;
    background-color: var(--rax-darkest);
    padding-top: 12.5rem;
}

/* // Utylity */
section {
    width: 100%;
    background-size: cover;
    background-position: center;
    color: var(--rax-light);
}


.half_container {
    width: 50%;
    height: 100%;
    padding: 2.5rem;
    /* border: 1px solid white; */
}

.half_container.right_to_center {
    justify-content: flex-end;
}


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
</style>