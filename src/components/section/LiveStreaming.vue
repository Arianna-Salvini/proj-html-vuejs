<script>
import ButtonBack from "../elements/ButtonBack.vue";
import ButtonNext from "../elements/ButtonNext.vue";
import SectionTitle from "../elements/SectionTitle.vue";


export default {
    name: 'LiveStreaming',
    components: {
        ButtonBack,
        ButtonNext,
        SectionTitle,
    },
}
</script>

<template>
    <section class="live_streaming overlay">
        <div class="half_container"></div>
        <div class="half_container">
            <div class="top">
                <SectionTitle title="Checkout our llive streaming" titleSection="Live Streaming" />
            </div>
            <div class="bottom thumbnails">
                <div class="button_box">
                    <ButtonBack />
                    <ButtonNext />
                </div>
                <!-- /.button_box -->
            </div>
            <!-- /.bottom card_miniature -->
        </div>
    </section>

</template>

<style></style>