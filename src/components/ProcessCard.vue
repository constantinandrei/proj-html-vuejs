<template>
    <div class="col">
        <div class="pt-2 pb-5 text-center">
            <div class="square m-auto d-flex align-items-center justify-content-center" :style="{color: iconColor}">
                <font-awesome-icon :icon="iconClass" />
            </div>
            <div class="my-card-title py-3">
                {{cardTitle}}
            </div>
            <div class="my-card-text text-muted">
                {{cardText}}
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ProcessCard',
        props: {
            iconClass: String,
            iconColor: String,
            cardTitle: String,
            cardText: {
                type: String,
                default: 'Lorem ipsum dolor sit, conetu adipisc sed be et aliqua pleasure itself.'
            }
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

    .my-card-text {
        font-size: .7rem;
    }
</style>