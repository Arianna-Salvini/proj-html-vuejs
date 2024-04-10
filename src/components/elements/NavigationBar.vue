<script>
export default {
    name: 'NavigationBar',
    props: {
        menuVoices: Object,
    }
}
</script>

<template>
    <nav class="navbar d_flex">
        <!-- Logo Left -->
        <div class="logo">
            <img src="/img/menulogo.png" alt="">
        </div>
        <!-- Navigation Element -->
        <ul class="menu_nav d_flex">
            <li v-for="(menuVoice, index) in menuVoices" :key="index">
                <a>{{ menuVoice.title }}</a>
            </li>
        </ul>
        <!-- Right Icon  -->
        <div class="d_flex ">
            <div class="icon_menu d_flex">
                <i class="fa-solid fa-magnifying-glass"></i>
            </div>
            <div class="icon_menu d_flex">
                <i class="fa-solid fa-bag-shopping"></i>
            </div>
        </div>
    </nav>
</template>

<style>
.navbar {
    height: 6rem;
    padding: 1rem;
    justify-content: space-between;

    .logo {
        height: 100%;
    }

    .menu_nav {
        padding: 1rem;
        width: 70%;
        justify-content: center;



        &>li {
            padding: 1rem;
            list-style-type: none;
        }
    }

    .menu_nav a {
        text-decoration: none;
        font-size: 1rem;
        text-transform: uppercase;
        color: var(--rax-light);

    }

    .icon_menu {
        width: 3rem;
        height: 3rem;
        color: var(--rax-darkest);
        background-color: var(--rax-light);
        border-radius: 50%;
        justify-content: center;
        margin-right: 1rem;
        position: relative;
    }
}

/* DropdownMenu */
/* 
.dropdown_menu {
    position: absolute;
    background-color: var(--rax-darker);
    padding: 0.5rem;
    border-bottom: 1px solid var(--rax-secondary);
    z-index: 1000;
    display: none;
}

.dropdown_menu ul {
    list-style-type: none;
}

.dropdown_menu ul li {
    padding: 1rem;
}

.dropdown_menu ul li a {
    text-decoration: none;
    color: var(--rax-secondary);
}

.dropdown_menu li:hover {
    display: block;
} */
</style>
