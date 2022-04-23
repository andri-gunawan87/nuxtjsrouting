<template>
  
  <div class="card m-4 " style="width: 18rem;">
  <img :src="article.img" class="card-img-top" alt="#">
  <div class="card-body">
    <nuxt-link class="title-task mb-1" :to="'app/detail/' + article.id">
    <h5 class="card-title">{{ article.title }}</h5>
    </nuxt-link>
    <p class="card-text">{{ article.content}}</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
</template>

<script>
export default {
  props: {
    article: {
      type: Object,
    },
  },
};
</script>

<style scoped>
.article-img img {
  width: 100%;
}
</style>