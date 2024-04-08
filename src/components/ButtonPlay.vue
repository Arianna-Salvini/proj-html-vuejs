<script>
export default {
    name: 'ButtonPlay',
}
</script>

<template>
    <button class="play_btn">
        <div class="play_btn_icon">
            <i class="fa-solid fa-play"></i>
        </div>
    </button>
</template>

<style scoped>
.play_btn {
    width: 3.3rem;
    aspect-ratio: 1;
    color: var(--rax-darkest);
    background-color: var(--rax-secondary);
    border-radius: 50%;
    border: none;

    .play_btn_icon {
        font-size: 1rem;
    }

}

.play_btn:hover {
    background-color: transparent;
    border: 1px solid var(--rax-secondary);
    color: var(--rax-secondary);
}
</style>
