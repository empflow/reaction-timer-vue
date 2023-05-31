<template>
  <Header />
  <button @click="start">Play</button>
</template>


<script lang="ts">
import { defineComponent } from 'vue';
import Header from './components/Header.vue';


export default defineComponent({
  data() {
    return {
      isPlaying: false
    }
  },
  methods: {
    start() {
      this.isPlaying = !this.isPlaying;
    }
  },
  components: { Header }
})
</script>
