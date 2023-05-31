<template>
  <div class="component">
    <h2>this is the component</h2>
    <p>Data: {{ data }}</p>
  </div>
</template>


<script lang="ts">
import { defineComponent } from 'vue';


export default defineComponent({
  props: ["data"]
})
</script>