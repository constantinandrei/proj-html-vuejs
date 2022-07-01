<template>
    <nav class="navbar">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">
                <img src="img/logo-sidearea-1.png" alt="">
            </a>
            <div class="d-flex">
                <ul class="navbar-nav ms-auto flex-row gap-3">
                <li v-for="link in navLinks" :key="link" class="nav-item">
                    <a class="nav-link text-black" href="#">{{link}}</a>
                </li>
            </ul>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'TheNav',
        data(){
            return {
                navLinks: ['HOME', 'PAGES', 'PORTFOLIO', 'BLOG', 'SHOP', 'ELEMENTS']
            }
        }
    }
</script>

<style lang="scss" scoped>
    nav {
        background-color: rgb(255, 255, 255);
        z-index: 5;
        position: sticky;
        top: 0;

        .navbar-brand {
            img {
                width: 100px;
            }
        }
    }
</style>