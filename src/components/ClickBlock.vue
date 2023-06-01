<template>
  <div class="click-block">
    <div class="icons">
      <img v-show="showLightningIcon" src="@/assets/lightningBolt.svg" class="icon" />
      <img v-show="showWaitIcon" src="@/assets/wait.svg" class="icon" />
      <img v-show="showCursorIcon" src="@/assets/cursor.svg" class="icon" />
      <img v-show="showCautionIcon" src="@/assets/caution.svg" class="icon" />
    </div>

    <div class="big-text">

    </div>

    <div class="small-text">

    </div>
    <button @click="toggleLightningIcon">lightning bolt icon</button><br />
    <button @click="toggleWaitIcon">wait icon</button><br />
    <button @click="toggleCursorIcon">cursor icon</button><br />
    <button @click="toggleCautionIcon">caution icon</button><br />
    <AiAcademia />
  </div>
</template>


<script lang="ts">
import { defineComponent } from 'vue';
import Icon from "oh-vue-icons";
import { AiAcademia } from "oh-vue-icons/icons";


export default defineComponent({
  name: "ClickBlock",
  data() {
    return {
      playing: false,
      clickedTooSoon: false,
      finished: false,
      showLightningIcon: false,
      showCursorIcon: false,
      showWaitIcon: false,
      showCautionIcon: false
    }
  },
  components: { "v-icon": Icon },
  methods: {
    toggleLightningIcon() {
      this.showLightningIcon = !this.showLightningIcon;
    },
    toggleCursorIcon() {
      this.showCursorIcon = !this.showCursorIcon;
    },
    toggleWaitIcon() {
      this.showWaitIcon = !this.showWaitIcon;
    },
    toggleCautionIcon() {
      this.showCautionIcon = !this.showCautionIcon;
    }
  },
})
</script>


<style>
.icon {
  color: red;
  background-color: red;
  border: 1px solid black;
  max-width: 100px;
}
</style>
