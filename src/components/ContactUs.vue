<template>
    <div class="section position-relative">
        <div class="position-absolute">
            <img src="img/send-message.png" alt="">
        </div>
        <div class="container h-100 position-relative">
            <div class="d-flex h-100 align-items-center text-center">
                <div class="col">
                    <h2 class="mb-3">Want to work with us? Send us <span>a message!</span></h2>
                    <p class="text-muted mb-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam officia possimus consequuntur nisi, nemo harum quasi tempore sapiente deleniti cumque. Quo iusto aliquid voluptate. Odit illo eius laboriosam explicabo corporis!</p>
                    <div class="btn btn-primary">CONTACT</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ContactUs'
    }
</script>

<style lang="scss" scoped>
    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    h2 {
        font-size: 3rem;

        span {
            font-style: italic;
            font-weight: bold;
            font-family: 'Comic Sans MS';
        }
    }
    .section {
        height: 530px;
    }
    .position-relative {
        z-index: 3;
    }
    .position-absolute{
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
    }
</style>