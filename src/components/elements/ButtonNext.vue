<script>
export default {
    name: 'ButtonNext',
}
</script>

<template>
    <button class="next_btn">
        <div class="btn_icon">
            <i class="fa-solid fa-arrow-right-long"></i>
        </div>
    </button>
</template>

<style scoped>
.next_btn {
    width: 3.3rem;
    aspect-ratio: 1;
    color: var(--rax-darkest);
    background-color: var(--rax-light);
    border-radius: 50%;
    border: none;
    margin: 0 0.5rem;

    .btn_icon {
        font-size: 1rem;
    }

}

.next_btn:hover {
    background-color: var(--rax-highlight);
    color: var(--rax-light);
}
</style>