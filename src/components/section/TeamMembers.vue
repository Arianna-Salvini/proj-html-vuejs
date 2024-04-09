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
            <div class="bottom_section">

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

/* Style */

.half_container {
    width: 50%;
    height: 100%;
    padding: 7rem 0;

    .button_box {
        justify-content: flex-end;
    }

    .bottom_section {
        width: 300px;
        height: 390px;
    }
}
</style>
