<template>
  <div class="root">
    <h1>this is the root component</h1>
    <p>dynamic data: {{  someData  }}</p>
  </div>

  <Component data="hiiiiii" />
</template>


<script lang="ts">
import { defineComponent } from 'vue';
import Component from './components/Component.vue';

export default defineComponent({
  data() {
    return {
      someData: "hello"
    }
  },
  components: {
    Component
  }
})
</script>


<style scoped>
.root {
  padding: 10px 15px;
  border: 3px solid green;
  border-radius: 5px;
}
</style>