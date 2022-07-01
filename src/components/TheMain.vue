<template>
    <main>
        <ImageSection></ImageSection>
        <WorkingProcess></WorkingProcess>
    </main>
</template>

<script>
import ImageSection from './ImageSection.vue';
import WorkingProcess from './WorkingProcess.vue';

    export default {
    name: "TheMain",
    components: { ImageSection, WorkingProcess }
}
</script>