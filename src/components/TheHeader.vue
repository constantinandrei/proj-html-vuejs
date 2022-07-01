<template>
    <div class="section position-relative p-5">
        <div class="container">
            <div class="row row-cols-2">
                <div class="col row align-items-center">
                    <div class="col">
                        <div class="p-5">
                            <h1 class="letter-spacing">Devotion thad never <span>ends</span></h1>
                            <p class="text-muted py-3">Nesque porro quisquantum est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi.</p>
                            <div class="btn btn-outline">READ MORE</div>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="p-5 h-100">
                        <JumboImage></JumboImage>
                    </div>
                </div>
            </div>
            <div class="row w-25 align-items-center justify-content-center m-auto">
                <div v-for="(num, i) in 3" :key="'point' + num"  class="col col-1">
                    <div class="slider-point" :class="{'active' : i === 2}"></div>
                </div>
                
            </div>
        </div>
        <div class="slider-arrow left">
            <font-awesome-icon icon="fa-solid fa-chevron-left" />
        </div>
        <div class="slider-arrow right">
            <font-awesome-icon icon="fa-solid fa-chevron-right" />
        </div>
    </div>
</template>

<script>
import JumboImage from './JumboImage.vue';
    export default {
    name: "TheHeader",
    components: { JumboImage }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

    h1 {
        font-weight: 400;
        font-size: 4rem;

        span {
            font-weight: bold;
            font-style: italic;
        }
    }

    .slider-point{
        width: 7px;
        height: 7px;
        border-radius: 3px;
        background-color: $secondary;
        cursor: pointer;

        &.active {
            transform: scale(1.5);
        }
    }

    .slider-arrow {
        background-color: $secondary;
        border-radius: 50%;
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        height: 20px;
        width: 20px;
        color: white;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: .7rem;
        cursor: pointer;
        &.left {
            left: 30px;
        }

        &.right {
            right: 30px;
        }
    }



</style>