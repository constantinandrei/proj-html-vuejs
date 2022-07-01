<template>
    <div class="section py-5">
        <div class="container">
            <div class="py-5">
                <div class="py-5">
                    <div class="row row-cols-3">
                    <BlogCard :img-src="'h-2-blog-img-1.jpg'"
                        :article-title="'This way, loves: a detailed guide through new design'"></BlogCard>
                    <BlogCard :img-src="'h-2-blog-img-2.jpg'"
                        :article-title="'I try to give people a different way of looking art'"></BlogCard>
                    <BlogCard :img-src="'h-2-blog-img-3.jpg'"
                        :article-title="'Introduce Richard Laperrière of those amazing features'"></BlogCard>
                </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import BlogCard from './BlogCard.vue';
    export default {
    name: "BlogPosts",
    components: { BlogCard }
}
</script>

<style lang="ssss" scoped>

</style>