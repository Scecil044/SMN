<template>
  <div class="container max-w-4xl mx-auto flex">
    <div class="w-1/3">
      <img
        class="w-full rounded h-auto shadow-lg"
        src="https://via.placeholder.com/500"
        alt=""
      />
    </div>
    <div class="w-full pl-4">
      <div class="flex">
        <div class="w-1/2">
          <h1 class="text-2xl md-text-4xl text-left text-gray-900">John Doe</h1>
          <span class="text-md text-gray-900">London uk</span>
        </div>

        <div class="w-1/2 mt-2">
          <RouterLinkButton btnText="Edit profile" />
        </div>
      </div>
      <ProfileInfoSection />
      <AboutSection />
    </div>
  </div>
</template>
<script setup>
import ProfileInfoSection from "@/components/partials/ProfileInfoSection.vue";
import AboutSection from "@/components/partials/AboutSection.vue";
import RouterLinkButton from "@/components/global/RouterLinkButton.vue";
</script>
