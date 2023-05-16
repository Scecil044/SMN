<template>
  <div>
    <div class="mx-auto py-4">
      <div class="flex flex-wrap font-bold text-gray-100">
        <div class="text-xl text-gray-900">Songs</div>
        <div class="bg-green-500 w-full h-1"></div>
        <div class="w-full mt-4">
          <RouterLinkButton btnText="Delete" />
          <RouterLinkButton btnText="Add Song" />
        </div>
      </div>
    </div>
   
  </div>
</template>
<script setup>
import RouterLinkButton from "../global/RouterLinkButton.vue";
</script>
