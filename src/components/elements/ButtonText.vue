<script>
export default {
    props: {
        title: String,
        iconButton: String,
    }
}
</script>

<template>
    <button class="text_button">
        <span class="title_button">
            {{ title }}
        </span>
        <!-- Aggiungo la favicon quando serve -->
        <i v-if="iconButton" :class="iconButton"></i>
    </button>
</template>

<style>
.text_button {
    margin-right: 2rem;
    padding: 1rem 2rem;
    font-size: 1rem;
    color: var(--rax-darkest);
    background-color: var(--rax-secondary);
    border-radius: 0.5rem;
    border: none;


    .title_button {
        padding-right: 0.3rem;
    }
}

button:hover {
    background-color: transparent;
    border: 1px solid var(--rax-secondary);
    color: var(--rax-secondary);
}
</style>
