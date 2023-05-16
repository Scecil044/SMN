<template>
  <div id="register">
    <div class="w-full p-6 flex items-center justify-center">
      <div class="w-full max-w-xs">
        <div class="p-6 rounded shadow-md bg-black mb-4">
          <h1 class="text-gray-200 text-lg mb-3 font-thin">Lets Get Rocking</h1>

          <div class="mb-4">
            <InputField
              placeholder="Eamil"
              v-model:input="email"
              inputType="text"
              label="Email"
              :labelColor="false"
              error="this is a test error"
            />
          </div>

          <div class="mb-4">
            <InputField
              placeholder="Password"
              v-model:input="password"
              inputType="password"
              label="Password"
              :labelColor="false"
              error="this is a test error"
            />
          </div>

          <button
            type="submit"
            class="block bg-green-500 text-sm text-white py-2 px-4 w-full rounded"
            @click="login"
          >
            Register
          </button>
        </div>
        <p class="text-center">
          Don't have an account?
          <router-link to="register" class="text-blue-600"
            >Register</router-link
          >
        </p>
      </div>
    </div>
  </div>
</template>
<script setup>
import InputField from "@/components/global/InputField.vue";

import { ref } from "vue";

let email = ref(null);
let password = ref(null);
</script>
<style scoped></style>
