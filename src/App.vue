<template>
  <h1>Reaction Timer</h1>
  <button @click="start">Play</button>
</template>


<script lang="ts">
import { defineComponent } from 'vue';


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
  components: {}
})
</script>
