<template>
  <dialog ref="dialogRef">
    <h3>Dialog opened</h3>
    <p>Try to inspect element below with vue-devtools inspector:</p>
    <DialogChild />
    <button @click="$emit('close')">Close</button>
  </dialog>
</template>

<script setup>
import { onMounted, ref } from "vue";
import DialogChild from "./DialogChild";

const dialogRef = ref();

onMounted(() => {
  dialogRef.value.showModal();
});
</script>
