<template>
    <main>
        <ImageSection></ImageSection>
        <WorkingProcess></WorkingProcess>
        <ContactUs></ContactUs>
    </main>
</template>

<script>
import ImageSection from './ImageSection.vue';
import WorkingProcess from './WorkingProcess.vue';
import ContactUs from './ContactUs.vue';

    export default {
    name: "TheMain",
    components: { ImageSection, WorkingProcess, ContactUs }
}
</script>