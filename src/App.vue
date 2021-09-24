<template>
  <div class="w-screen h-screen flex items-center justify-center bg-gray-50 dark:bg-gray-900 px-5" >
    <div class="bg-white dark:bg-gray-800 shadow-xl w-full lg:w-4/12 md:w-8/12 sm:w-10/12 p-6">
      <h4 class="font-semibold mb-3 border-b border-gray-200 dark:text-gray-200">login</h4>
      <div class="space-y-3">
        <input
          class="px-3 py-2 placeholder-gray-300 border-gray-300 dark-border-800 w-full dark:bg-gray-600 dark:text-gray-200"
          type="text"
          placeholder="E-mail"
        />

        <input
          class="px-3 py-2 placeholder-gray-300 border-gray-300 dark-border-800 w-full dark:bg-gray-600 dark:text-gray-200"
          type="text"
          placeholder="Senha"
        />
        <div class="text-right">
          <button
            class="
              rounded
              text-sm
              px-3
              py-2
              bg-green-400
              hover:bg-green-800
              tex-green-900
            "
          >
            login
          </button>
        </div>
      </div>
    </div>
  </div>
  <DarkModeSwitch/>
</template>

<script>
import DarkModeSwitch from './components/DarkModeSwitch.vue';
import HelloWorld from "./components/HelloWorld.vue";

export default {
  components: { DarkModeSwitch },
  name: "App",
};
</script>


