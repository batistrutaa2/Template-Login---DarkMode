<template>
  <div
    class="absolute top-0 right-0 p-4 cursor-pointer dark:text-gray-300"
    @click="toggle"
  >
    {{ name }}
  </div>
</template>

<script>
export default {
  name: "DarkModeSwitch",
  data() {
    return {
      isDark: false,
    };
  },

  computed: {
    name() {
      return this.isDark ? "light" : "Dark";
    },
  },

  watch: {
    isDark(vl) {
      const htmlel = document.getElementsByTagName("html")[0];
      if (vl) {
        htmlel.classList.add("dark");
      } else {
        htmlel.classList.remove("dark");
      }
    },
  },

  methods: {
    toggle() {
      this.isDark = !this.isDark;
    },
  },
};
</script>

<style>
</style>