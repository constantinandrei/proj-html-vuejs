<template>
    <div class="col">
        <div class="py-2">
            <div class="square m-auto d-flex align-items-center justify-content-center" :style="{color: iconColor}">
            <font-awesome-icon :icon="iconClass" />
        </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ProcessCard',
        props: {
            iconClass: String,
            iconColor: String
        }
    }
</script>

<style lang="scss" scoped>
    .square {
        width: 50%;
        aspect-ratio: 1 / 1;
        background-color: rgb(250, 247, 241);
        border-radius: 50%;
        position: relative;
        z-index: 1;
        font-size: 2rem;
    }
</style>