<template>
    <div class="post-container">
        <post-card v-for="post in posts" :key="post.title"
            :title="post.title"
            :summary="post.summary"
            :text="post.text"
        />
    </div>
</template>

<script lang="ts">
import { defineComponent, DefineComponent } from 'vue';
import PostCard from './PostCard.vue';
import datos from "@/assets/posts.json"

export default defineComponent({
    name: "PostContainer",
    components: {
        PostCard
    },
    computed: {
        posts : ()=>{
            return datos.map((post:any)=>{
                return post
            })
        }
    }
})
</script>

<style lang="scss" scoped>
    .post-container {
        width: 100%;
        display: flex;
        flex-wrap: wrap;
    }
</style>