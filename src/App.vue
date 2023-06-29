<template>
  <div>
    <div>Likes: <strong>{{ likes }}</strong></div>
    <div>Dislikes: <strong>{{ dislikes }}</strong></div>
    <button v-on:click="addLike">like</button>
    <button v-on:click="addDisLike">dislike</button>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        likes: 0,
        dislikes: 0,
      }
    },

    methods: {
      addLike() {
        this.likes += 1;
      },
      addDisLike() {
        this.dislikes += 1;
      }
    }
  }
</script>

<style>

</style>