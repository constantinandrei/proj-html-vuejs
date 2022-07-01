<template>
    <div class="py-1">
        <div class="row row-cols-3 g-0">
            <div v-for="num in 6" :key="num" class="col">
                <img :src="`img/h-2-port-img-${num}.jpg`" alt="">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ImageSection'
    }
</script>

<style lang="scss" scoped>
    img {
        width: 100%;
    }
</style>