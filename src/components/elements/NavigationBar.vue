<script>
export default {
    name: 'NavigationBar',
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
            <li>
                <a href="#">
                    Home <i class="fa fa-chevron-down" aria-hidden="true"></i>
                </a>
                <!-- <div class="dropdown_menu">
                            Home
                        </div> -->
            </li>
            <li>
                <a href="#">
                    Pages <i class="fa fa-chevron-down" aria-hidden="true"></i>
                </a>
                <!-- <div class="dropdown_menu">
                            Pages
                        </div> -->
            </li>
            <li>
                <a href="#">
                    Tournament
                </a>
            </li>
            <li>
                <a href="#">
                    Shop <i class="fa fa-chevron-down" aria-hidden="true"></i>
                </a>
                <!-- <div class="dropdown_menu">
                            Shop
                        </div> -->
            </li>
            <li>
                <a href="#">
                    Blog <i class="fa fa-chevron-down" aria-hidden="true"></i>
                </a>
                <!-- <div class="dropdown_menu">
                            Blog
                        </div> -->
            </li>
            <li>
                <a href="#">
                    Contact
                </a>
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
        list-style: none;
        width: 70%;
        justify-content: center;

        & a {
            text-decoration: none;
            font-size: 1rem;
            text-transform: uppercase;
            color: var(--rax-light);
        }

        &>li {
            padding: 1rem
        }

    }

    .icon_menu {
        width: 3rem;
        height: 3rem;
        background-color: var(--rax-light);
        border-radius: 50%;
        justify-content: center;
        margin-right: 1rem;

        &>i {
            color: var(--rax-darkest);
        }
    }
}
</style>
