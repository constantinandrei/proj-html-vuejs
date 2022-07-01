<template>
    <div class="h-100 position-relative">
        <img class="woman" src="img/h-2-slider-img-15.png" alt="">
        <img class="man" src="img/h-2-slider-img-16.png" alt="">
    </div>
</template>

<script>
    export default {
        name: 'JumboImage'
    }
</script>

<style lang="scss" scoped>
    img {
        position: absolute;
        height: 100%;
    }

    .woman {
        top: 0;
        left: 0;
        bottom: 0;
    }

    .man {
        top: 0;
        bottom: 0;
        right: 0;
    }
</style>