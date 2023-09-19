<template>
  <div>
    <h3>Open modal dialog below:</h3>
    <button @click="isDialogVisible = true">open dialog</button>
  </div>
  <HtmlBasedDialog v-if="isDialogVisible" @close="isDialogVisible = false" />
</template>

<script setup>
  import { ref } from 'vue';
  import HtmlBasedDialog from './HtmlBasedDialog.vue';
  
  const isDialogVisible = ref(false);
</script>
