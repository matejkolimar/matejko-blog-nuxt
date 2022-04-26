<template>
    <div>
        <section class="post-list">
            <PostPreview
                id="1"
                :is-admin="isAdmin"
                thumbnail="https://www.wpbeginner.com/wp-content/uploads/2020/04/featuredimageswp-og.png"
                title="Hello there!"
                preview-text="This is my first post!" />
            <PostPreview
                id="1"
                :is-admin="isAdmin"
                thumbnail="https://www.wpbeginner.com/wp-content/uploads/2020/04/featuredimageswp-og.png"
                title="Hello there!"
                preview-text="This is my second post!" />
            <PostPreview
                id="1"
                :is-admin="isAdmin"
                thumbnail="https://www.wpbeginner.com/wp-content/uploads/2020/04/featuredimageswp-og.png"
                title="Hello there!"
                preview-text="This is my third post!" />
        </section>
    </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview.vue'
export default {
    components: {
        PostPreview,
    },
    props: {
        isAdmin: {
            type: Boolean,
            default: false,
        },
    },
}
</script>

<style scoped>
.post-list {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}
</style>
