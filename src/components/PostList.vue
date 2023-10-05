<template>
     <div class="post" v-for="post in posts" :key="post.id">
        <div>Название:<strong> {{ post.title }}</strong></div>
        <div>Описание:<strong> {{ post.body }}</strong></div>
    </div>
</template>

<script>
export default {
    props: {
        posts: {
            type: Array,
            required: true,
        }
    }
}
</script>

<style>
    .post{
        padding: 15px;
        border: 2px solid teal;
        margin-top: 15px;
    }
</style>