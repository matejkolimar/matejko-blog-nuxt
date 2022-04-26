<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost" />
        </section>
    </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm.vue'

export default {
    components: {
        AdminPostForm,
    },
    layout: 'admin',
    data() {
        return {
            loadedPost: {
                author: 'Maximilian',
                title: 'My awesome Post',
                content: 'Super amazing, thanks for that!',
                thumbnailLink:
                    'https://www.wpbeginner.com/wp-content/uploads/2020/04/featuredimageswp-og.png',
            },
        }
    },
}
</script>
<style scoped>
.update-form {
    width: 90%;
    margin: 20px auto;
}
@media (min-width: 768px) {
    .update-form {
        width: 500px;
    }
}
</style>
