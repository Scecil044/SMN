<template>
  <div class="w-7xl mx-auto">
    <form action="" class="mt-24">
      <NewInput
        placeholder="Email"
        label="email"
        type="email"
        v-model="email"
      />
    </form>
  </div>
</template>
<script setup>
import { ref } from "vue";
import NewInput from "@/components/global/NewInput.vue";

const email = ref("");
</script>
<style scoped></style>
