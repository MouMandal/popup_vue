<script setup>
import { ref } from 'vue';
const content = ref(true);
const popups = () => {
  content.value = false;
}
</script>

<template>
  <div class="container">
    <div v-if="content" class="popup">
      <h2>Are You Sure?</h2>
      <p>you want to delete this song</p>
      <div class="bts">
        <button @click="popups" id="btn">Yes</button>
        <button id="btn_1">No</button>
      </div>

    </div>
  </div>
</template>

<style scoped></style>
