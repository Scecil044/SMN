<template>
  <div>
    <label for="">
      {{ label }}
    </label>
    <input :type="type" :placeholder="placeholder" v-model="computeInput" />
  </div>
</template>
<script setup>
import { computed, defineProps, defineEmits } from "vue";

const emit = defineEmits(["update:input"]);
const props = defineProps({
  placeholder: String,
  input: String,
  type: String,
  label: String,
});

const computeInput = computed({
  get: () => props.input,
  set: (value) => emit("update:input", value),
});
</script>
<style scoped></style>
