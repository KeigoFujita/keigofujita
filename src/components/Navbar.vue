<template>
  <nav class="px-5 md:px-12">
    <div class="flex flex-col md:flex-row justify-center md:justify-between items-center pt-10">
      <router-link :to="{name:'home'}">
        <div class="flex items-center mb-5 md:mb-0">
          <img src="@/assets/img/logo.png" alt srcset class="w-12 h-12 mr-3" />
          <h1 class="text-4xl font-semibold md:text-4xl font-orbitron dark:text-white">
            <span class="font-bold text-primary dark:text-white">keigo</span>fujita
          </h1>
        </div>
      </router-link>
      <div class="flex font-sans justify-center dark:text-white">
        <button class="h-6 w-6 mr-2 focus:outline-none" @click="toggleDark">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            v-show="this.$parent.theme == 'light'"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"
            />
          </svg>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            v-show="this.$parent.theme == 'dark'"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z"
            />
          </svg>
        </button>

        <router-link
          class="px-2 font-bold text-gray-800 dark:text-white"
          :to="{name:'projects'}"
        >PROJECTS</router-link>
        <router-link
          class="px-2 font-bold text-gray-800 dark:text-white"
          :to="{name:'contact'}"
        >CONTACT</router-link>
      </div>
    </div>
  </nav>
</template>

<script>
export default {

  methods : {
     toggleDark : function() {
        this.$parent.theme = this.$parent.theme == 'light' ? 'dark' : 'light';
        localStorage.setItem('theme',this.$parent.theme)
     }
  }
}
</script>