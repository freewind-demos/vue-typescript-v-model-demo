<template>
  <div class="hello">
    <input type="text" v-model="message"/>
    <button type="button" @click="showMessage1">Show Correct</button>
    <button type="button" @click="showMessage2">Show Invalid</button>
  </div>
</template>

<script lang="ts">
  import {Component, Vue} from 'vue-property-decorator';

  @Component
  export default class HelloWorld extends Vue {
    message = "change me";
    showMessage1() {
      alert(this.message)
    }
    showMessage2 = () => {
      alert(this.message)
    }
  }
</script>

<style scoped>
  .hello {
    color: red;
  }
</style>
