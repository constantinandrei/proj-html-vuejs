<template>
    <div class="pt-3 pb-5">
        <div class="container">
            <h2 class="text-center py-5">Working <span>process</span></h2>
            <div class="w-75 m-auto position-relative">
                <div class="row row-cols-4">
                    <ProcessCard
                    :icon-class="'fa-solid fa-lightbulb'"
                    :icon-color="'#BADAC9'"
                    :card-title="'First there\'s an idea'" ></ProcessCard>
                    <ProcessCard
                    :icon-class="'fa-regular fa-comment'"
                    :icon-color="'#F8D12D'"
                    :card-title="'Then we talk about'" ></ProcessCard>
                    <ProcessCard
                    :icon-class="'fa-solid fa-cloud'"
                    :icon-color="'#80465F'"
                    :card-title="'And we think about'" ></ProcessCard>
                    <ProcessCard
                    :icon-class="'fa-solid fa-pencil'"
                    :icon-color="'#EB6950'"
                    :card-title="'So we draw along'" ></ProcessCard>
                </div>
                <div class="my-position-absolute">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1095.3 126">
                        <path
                            d="M2.3 58s70 50.4 177 52c101.5 1.5 145.1-20.7 170-31.8 5.9-2.6 38.9-20.5 38.9-20.5 3.8-2.8 72.7-43.4 159.4-43.7s132.1 29.3 162.3 45.4c0 0 26.6 14.5 36.7 19.3 2.9 1.4 64.7 29.3 169.7 30.3s166-46.3 178-50"
                            fill="none" stroke-width="2" stroke="#f1cfc6" />
                    </svg>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import ProcessCard from './ProcessCard.vue';
    export default {
    name: "WorkingProcess",
    components: { ProcessCard }
}
</script>

<style lang="scss" scoped>
    .my-position-absolute {
        position: absolute;
        top: 0;
        right: 8%;
        bottom: 0;
        left: 8%;
    }

    h2 {
        font-size: 3rem;

        span {
            font-family: 'Comic Sans MS';
            font-weight: bold;
            font-style: italic;
        }
    }
</style>