<template>
    <main>
        <ImageSection></ImageSection>
        <WorkingProcess></WorkingProcess>
        <ContactUs></ContactUs>
        <BlogPosts></BlogPosts>
    </main>
</template>

<script>
import ImageSection from './ImageSection.vue';
import WorkingProcess from './WorkingProcess.vue';
import ContactUs from './ContactUs.vue';
import BlogPosts from './BlogPosts.vue';

    export default {
    name: "TheMain",
    components: { ImageSection, WorkingProcess, ContactUs, BlogPosts }
}
</script>