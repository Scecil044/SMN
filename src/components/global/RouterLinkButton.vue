<template>
  <royter-link
    :to="url"
    class="text-gray-900 float-right bg-transparent py-2 px-4 font-semibold border border:hover-transparent rounded hover:bg-green-700 hover:text-white border-green-500"
    >{{ btnText }}</royter-link
  >
</template>
<script setup>
import { defineProps, toRefs } from "vue";
const props = defineProps({
  btnText: String,
  url: String,
  //   color: String,
});
const { btnText, url } = toRefs(props);
</script>

<style scoped></style>
