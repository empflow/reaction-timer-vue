<template>
  <div class="header">
    <h1 class="title">Reaction Timer</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({

})
</script>

<style>
.header {
  display: flex;
  justify-content: center;
}

.header .title {
  text-align: center;
  font-size: 1.5rem;
  font-weight: 600;
  padding: 10px;
  width: 100%;
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.1)
}
</style>