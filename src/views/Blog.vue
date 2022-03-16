<template>
  <div>
    <h2>Blog</h2>

    <!-- <input type="checkbox" value="checked" v-model="isChecked" /> -->
    <button @click="showParagraph">Mostrar</button>
    <h1 v-if="show">Conditional rendering is really cool!</h1>
    <h1 v-else-if="counter">My counter is 3</h1>
    <h1 v-else>Oh no</h1>
  </div>
</template>

<script>
import Article from "../components/Article.vue";
export default {
  components: {
    Article,
  },
  data() {
    return {
      show: false,
      counter: 3,
    };
  },
  methods: {
    showParagraph() {
      this.show = !this.show;
    },
  },
};
</script>

<style></style>
