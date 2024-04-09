<script>
export default {
    name: 'ButtonBack',
}
</script>

<template>
    <button class="play_btn">
        <div class="play_btn_icon">
            <i class="fa-solid fa-arrow-left-long"></i>
        </div>
    </button>
</template>

<style scoped>
.play_btn {
    width: 3.3rem;
    aspect-ratio: 1;
    color: var(--rax-darkest);
    background-color: var(--rax-light);
    border-radius: 50%;
    border: none;
    margin: 0 0.5rem;

    .play_btn_icon {
        font-size: 1rem;
    }

}

.play_btn:hover {
    background-color: var(--rax-highlight);
    color: var(--rax-light);
}
</style>