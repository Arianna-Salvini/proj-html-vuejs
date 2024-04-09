<script>
export default {
    props: {
        titleSection: String,
        title: String,
    }
}
</script>

<template>
    <h5 class="section_title"> {{ titleSection }}</h5>
    <h2 class="title_text">{{ title }}</h2>
</template>

<style>
.section_title {
    color: var(--rax-secondary);
    text-transform: uppercase;
    font-size: 1rem;
    padding-bottom: 1.5rem;
}

.title_text {
    font-size: 2.9rem;
    text-transform: capitalize;
}
</style>