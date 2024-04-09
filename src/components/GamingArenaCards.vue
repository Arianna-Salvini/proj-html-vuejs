<script>
export default {
    props: {
        image: String,
        title: String,
        description: String,
    }
}
</script>

<template>
    <div class="gaming_arena_card ">
        <img class="card_img" :src="image" alt="">
        <h2 class="title_gaming_arena"> {{ title }} </h2>
        <div class="description"> {{ description }}</div>
    </div>
</template>

<style>
.gaming_arena_card {
    width: 310px;
    height: 320px;
    border-radius: 10px;
    background-color: var(--rax-primary);
    text-align: center;
    padding: 3rem, 2rem;
    line-height: 1.8rem;


    .card_img {
        width: 6.5rem;
        height: 6.5rem;
        background-color: var(--rax-darkest);
        border-radius: 50%;
        object-fit: scale-down;
        margin-top: 3rem;
    }

    .title_gaming_arena {
        padding-top: 1rem;
    }

    .description {
        font-weight: 100;

    }
}

.gaming_arena_card:hover {
    background-color: var(--rax-secondary);
    color: var(--rax-darkest);
}
</style>
