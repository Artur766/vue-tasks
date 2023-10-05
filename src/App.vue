<template>
    <div class="app">
        <PostForm></PostForm>
        <PostList :posts="posts"></PostList>
    </div>
</template>

<script>
import PostForm from '@/components/PostForm.vue';
import PostList from '@/components/PostList.vue';
export default {
    components: {
        PostForm, PostList
    },
    data() {
        return {
            posts: [
                { id: 1, title:"js1", body: "Описание"},
                { id: 2, title: "js2", body: "Описание" },
                { id: 3, title: "js3", body: "Описание" },
            ],
        }
    },
    methods:{
        createPost(){
          
        },
    }
}
</script>

<style >
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    .app{
        padding: 20px;
    }
  
</style>
