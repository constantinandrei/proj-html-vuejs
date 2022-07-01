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
                    <JumboImage></JumboImage>
                </div>
            </div>
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
    h1 {
        font-weight: 400;
        font-size: 4rem;

        span {
            font-weight: bold;
            font-style: italic;
        }
    }

</style>