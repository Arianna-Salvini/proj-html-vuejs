<script>
import SectionTitle from "../elements/SectionTitle.vue";
import GamingArenaCards from "../elements/GamingArenaCards.vue"


export default {
    name: 'GamingArena',
    components: {
        SectionTitle,
        GamingArenaCards
    },
    data() {
        return {
            cards: [
                { id: 1, image: '../../public/img/feature1.png', title: 'Live Streaming', description: 'Nulla porttitor accumsan tincidunt.Pellentesque in.' },
                { id: 2, image: '../../public/img/feature2.png', title: 'Gaming News', description: 'Nulla porttitor accumsan tincidunt.Pellentesque in.' },
                { id: 3, image: '../../public/img/feature3.png', title: 'Great tournament', description: 'Nulla porttitor accumsan tincidunt.Pellentesque in.' },
                { id: 4, image: '../../public/img/feature4.png', title: 'Award Ceremony', description: 'Nulla porttitor accumsan tincidunt.Pellentesque in.' },
            ]
        }
    }
}
</script>

<template>
    <section class="gaming_area d_flex">
        <div class="half_container right_to_center d_flex">
            <div class="text_box">
                <!-- Component for titles -->
                <div class="title_section">
                    <SectionTitle title="the best gaming arena on the world!" titleSection="Our Extrem Feature" />
                </div>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque aperiam aspernatur corporis illo
                    cupiditate commodi, architecto sequi provident pariatur temporibus sapiente sit praesentium iste
                    voluptate et odit vero dicta nihil harum, consequuntur molestiae dolore! Ut veritatis laudantium
                </p>
            </div>
        </div>
        <div class="hal_container d_flex">
            <div class="box_gaming_card d_flex">
                <GamingArenaCards v-for="card in cards" :key="card.id" :image="card.image" :title="card.title"
                    :description="card.description" />
            </div>
        </div>

    </section>
</template>

<style>
.half_container {
    width: 50%;
    height: 100%;
    padding: 2.5rem;
    /* border: 1px solid white; */
}

.half_container.right_to_center {
    justify-content: flex-end;
}

.gaming_area {
    height: 802px;
    background-image: url(public/img/Vector.png);
}

.box_gaming_card {
    width: 640px;
    height: 660px;
    flex-wrap: wrap;
    gap: 1rem;
}
</style>