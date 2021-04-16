<template>
  <div :class="{ 'dark' : this.theme == 'dark'}" class="transition-all relative" id="parent">
    <div class="flex flex-col overflow-hidden bg-white dark:bg-d-primary content-wrapper">
      <div class="bg-primary h-3 w-full dark:bg-d-secondary"></div>
      <Navbar />
      <transition 
        name="fade"
        mode="out-in">
        <router-view />
      </transition>
    </div>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
export default {
  components: {
    Navbar
  },
  created: function(){
    this.theme = localStorage.getItem('theme') || 'light';
  },
  data: function(){
    return{
      theme : 'light'
    }
  },
}
</script>