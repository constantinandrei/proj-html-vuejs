<template>
    <div class="py-1">
        <div class="row row-cols-3 g-0">
            <div v-for="text, i in hoverText" :key="'illustrate' + i" class="col">
                <div class="position-relative h-100 overflow-hidden">
                    <img :src="`img/h-2-port-img-${i + 1}.jpg`" alt="">
                    <div class="hover-text p-4">
                        <h5>{{text}}</h5>
                        <em>Illustration</em>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ImageSection',
        data(){
            return {
                hoverText: ['All These illustrations', 'Type and illustrations', 'Draw and illustrate', 'Illustrations of novels', 'Too many illustrations', 'Dreams are illustrations']
            }
        }
    }
</script>

<style lang="scss" scoped>
    img {
        width: 100%;
    }

    .position-relative:hover {

            .hover-text {
                transform: translate(0, -50%);
                opacity: 1;
            }
        }

    .hover-text {
        background-color: white;
        width: 50%;
        position: absolute;
        left: 0;
        top: 50%;
        transform: translate(-100%, -50%);
        transition: transform 400ms;
        overflow: hidden;
    }
</style>