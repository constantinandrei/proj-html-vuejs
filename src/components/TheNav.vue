<template>
    <nav class="navbar py-2 px-3">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">
                <img src="img/logo-sidearea-1.png" alt="">
            </a>

            <ul class="navbar-nav ms-auto flex-row gap-5 me-5">
                <li v-for="link in navLinks" :key="link" class="nav-item">
                    <a class="nav-link text-black" href="#">{{link}}</a>
                </li>
            </ul>
            <div class="img-container">
                <svg xmlns="http://www.w3.org/2000/svg" width="23" height="23">
                    <circle cx="3" cy="20.1" r="2" />
                    <circle cx="11.7" cy="20.1" r="2" />
                    <circle cx="20.2" cy="20.1" r="2" />
                    <circle cx="3" cy="2.9" r="2" />
                    <circle cx="11.7" cy="2.9" r="2" />
                    <circle cx="20.2" cy="2.9" r="2" />
                    <circle cx="3" cy="11.4" r="2" />
                    <circle cx="11.7" cy="11.4" r="2" />
                    <circle cx="20.2" cy="11.4" r="2" />
                </svg>
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
        font-size: .7rem;
        font-weight: bold;
        letter-spacing: 2px;

        .navbar-brand {
            img {
                width: 100px;
            }
        }
    }
</style>