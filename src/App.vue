<template>
  <div :class="{ 'dark' : this.theme == 'dark'}" class="transition-all relative" id="parent">
    <div class="absolute right-4 top-8 md:hidden flex items-center justify-center p-3 rounded dark:text-white">
      <button class="h-6 w-6 focus:outline-none" @click="toggleDark">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class=""
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              v-show="theme == 'light'"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"
              />
            </svg>
            <svg xmlns="http://www.w3.org/2000/svg" class="" fill="none" viewBox="0 0 24 24" stroke="currentColor" v-show="theme == 'dark'">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z" />
            </svg>
        </button>
    </div>
    <div class="flex flex-col overflow-hidden bg-white dark:bg-d-primary content-wrapper">
    <div class="bg-primary h-3 w-full dark:bg-d-secondary"></div>
    <div class="px-5 md:px-12">
      <div class="flex flex-col md:flex-row justify-center md:justify-between items-center pt-10">
        <div class="flex items-center mb-5 md:mb-0">
          <img src="./assets/img/logo.png" alt="" srcset="" class="w-12 h-12 mr-3">
          <h1 class="text-4xl font-semibold md:text-4xl font-orbitron dark:text-white">
          <span class="font-bold text-primary dark:text-white">keigo</span>fujita
        </h1>
        </div>
        <div class="flex font-sans justify-center dark:text-white">
          <button class="h-6 w-6 mr-2 hidden md:block focus:outline-none" @click="toggleDark">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class=""
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                v-show="theme == 'light'"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"
                />
              </svg>
              <svg xmlns="http://www.w3.org/2000/svg" class="" fill="none" viewBox="0 0 24 24" stroke="currentColor" v-show="theme == 'dark'">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z" />
              </svg>
          </button>
          <p class="px-2 font-bold text-gray-800 dark:text-white">PROJECTS</p>
          <p class="px-2 font-bold text-gray-800 dark:text-white">CONTACT</p>
        </div>
      </div>
    </div>
    <div class="mx-auto pt-24 px-2 w-full max-w-screen-md  font-open-sans">
      <div class="flex flex-col md:flex-row justify-between">
        <div class="text-center md:text-left">
          <h1
            class="text-4xl md:text-6xl font-bold md:font-semibold text-gray-800 mb-2 md:mb-6 dark:text-white"
          >Laravel web developer</h1>
          <h1
            class="text-primary text-2xl md:text-4xl font-bold md:font-semibold mb-10 dark:text-d-secondary"
          >Welcome to my website</h1>
        </div>
        <img src="./assets/svg/test.svg" alt srcset class="mx-auto w-64" />
      </div>
    </div>
    <div class="mx-auto pt-12 px-8 md:px-2 w-full max-w-screen-md font-open-sans">
      <p class="text-xl md:text-2xl dark:text-white">Hey, I'm Keigo. I create custom websites to help businesses do better online. I specialize in the Laravel PHP framework on the backend, Vue.js on the frontend and Tailwind CSS for styling. I also teach online where I share my knowledge and experience about Web Development.</p>
    </div>
    <div class="mx-auto py-12 px-8 w-full max-w-screen-md border-b border-gray-200 dark:border-white md:pt-20">
      <div class="flex flex-col md:flex-row justify-between items-center">
        <img src="./assets/svg/website.svg" alt class="w-5/6 sm:w-2/3 md:w-1/3 md:mb-0 mb-12 mx-auto" />
        <img src="./assets/svg/phone.svg" alt class="hidden md:w-1/3 md:block mx-auto" />
      </div>
    </div>
    <!-- PROJECTS -->
    <div class="mx-auto py-12 px-4 w-full max-w-screen-md border-b border-gray-200 dark:border-white font-open-sans relative">
      <p class="font-semibold text-gray-700 mb-5 md:text-xl dark:text-white">Here are some projects I've worked on:</p>
      <div class="flex items-stretch mb-4 md:text-xl">
        <div class="text-primary dark:text-d-secondary mr-5 py-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-8 w-8"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M6.267 3.455a3.066 3.066 0 001.745-.723 3.066 3.066 0 013.976 0 3.066 3.066 0 001.745.723 3.066 3.066 0 012.812 2.812c.051.643.304 1.254.723 1.745a3.066 3.066 0 010 3.976 3.066 3.066 0 00-.723 1.745 3.066 3.066 0 01-2.812 2.812 3.066 3.066 0 00-1.745.723 3.066 3.066 0 01-3.976 0 3.066 3.066 0 00-1.745-.723 3.066 3.066 0 01-2.812-2.812 3.066 3.066 0 00-.723-1.745 3.066 3.066 0 010-3.976 3.066 3.066 0 00.723-1.745 3.066 3.066 0 012.812-2.812zm7.44 5.252a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
        <div>
          <p class="text-gray-700 font-semibold dark:text-white">Sunpack ERP</p>
          <p
            class="text-gray-500 text-sm md:text-base dark:text-d-text-secondary"
          >An Enterprise Resource Planning software for a carton manufacturing company. Sunpack ERP integrates all software and business processes on a single system. Built with Powerbuilder and SQL Server.</p>
        </div>
      </div>
      <div class="flex items-stretch mb-4 md:text-xl">
        <div class="text-primary dark:text-d-secondary mr-5 py-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-8 w-8"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M6.267 3.455a3.066 3.066 0 001.745-.723 3.066 3.066 0 013.976 0 3.066 3.066 0 001.745.723 3.066 3.066 0 012.812 2.812c.051.643.304 1.254.723 1.745a3.066 3.066 0 010 3.976 3.066 3.066 0 00-.723 1.745 3.066 3.066 0 01-2.812 2.812 3.066 3.066 0 00-1.745.723 3.066 3.066 0 01-3.976 0 3.066 3.066 0 00-1.745-.723 3.066 3.066 0 01-2.812-2.812 3.066 3.066 0 00-.723-1.745 3.066 3.066 0 010-3.976 3.066 3.066 0 00.723-1.745 3.066 3.066 0 012.812-2.812zm7.44 5.252a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
        <div>
          <p class="text-gray-700 font-semibold dark:text-white">Gardner Clearance System</p>
          <p
            class="text-gray-500 text-sm md:text-base dark:text-d-text-secondary"
          >An efficient and computerized clearance system (web-based application) for the school. Gardner College Clearance System is capable of handling comprehensive information of the student in a simultaneous and speedy way.</p>
        </div>
      </div>
      <div class="flex items-stretch mb-4 md:text-xl">
        <div class="text-primary dark:text-d-secondary mr-5 py-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-8 w-8"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M6.267 3.455a3.066 3.066 0 001.745-.723 3.066 3.066 0 013.976 0 3.066 3.066 0 001.745.723 3.066 3.066 0 012.812 2.812c.051.643.304 1.254.723 1.745a3.066 3.066 0 010 3.976 3.066 3.066 0 00-.723 1.745 3.066 3.066 0 01-2.812 2.812 3.066 3.066 0 00-1.745.723 3.066 3.066 0 01-3.976 0 3.066 3.066 0 00-1.745-.723 3.066 3.066 0 01-2.812-2.812 3.066 3.066 0 00-.723-1.745 3.066 3.066 0 010-3.976 3.066 3.066 0 00.723-1.745 3.066 3.066 0 012.812-2.812zm7.44 5.252a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
        <div>
          <p class="text-gray-700 font-semibold dark:text-white">iVisit Lobby Management System</p>
          <p
            class="text-gray-500 text-sm md:text-base dark:text-d-text-secondary"
          >A desktop application for managing visitor entry and appointment. iVisit digitizes the traditional logbook process for obtaining visitor information. Built with Visual Basic and MySQL.</p>
        </div>
      </div>
      <div class="flex items-stretch mb-4 md:text-xl">
        <div class="text-primary dark:text-d-secondary mr-5 py-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-8 w-8"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M6.267 3.455a3.066 3.066 0 001.745-.723 3.066 3.066 0 013.976 0 3.066 3.066 0 001.745.723 3.066 3.066 0 012.812 2.812c.051.643.304 1.254.723 1.745a3.066 3.066 0 010 3.976 3.066 3.066 0 00-.723 1.745 3.066 3.066 0 01-2.812 2.812 3.066 3.066 0 00-1.745.723 3.066 3.066 0 01-3.976 0 3.066 3.066 0 00-1.745-.723 3.066 3.066 0 01-2.812-2.812 3.066 3.066 0 00-.723-1.745 3.066 3.066 0 010-3.976 3.066 3.066 0 00.723-1.745 3.066 3.066 0 012.812-2.812zm7.44 5.252a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
        <div>
          <p class="text-gray-700 font-semibold dark:text-white">Larabooks</p>
          <p
            class="text-gray-500 text-sm md:text-base dark:text-d-text-secondary"
          >A simple book management system built with Laravel. Larabooks has a built in REST API integration and authentication.</p>
        </div>
      </div>
      <div class="flex items-stretch md:text-xl">
        <div class="text-primary dark:text-d-secondary mr-5 py-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-8 w-8"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M6.267 3.455a3.066 3.066 0 001.745-.723 3.066 3.066 0 013.976 0 3.066 3.066 0 001.745.723 3.066 3.066 0 012.812 2.812c.051.643.304 1.254.723 1.745a3.066 3.066 0 010 3.976 3.066 3.066 0 00-.723 1.745 3.066 3.066 0 01-2.812 2.812 3.066 3.066 0 00-1.745.723 3.066 3.066 0 01-3.976 0 3.066 3.066 0 00-1.745-.723 3.066 3.066 0 01-2.812-2.812 3.066 3.066 0 00-.723-1.745 3.066 3.066 0 010-3.976 3.066 3.066 0 00.723-1.745 3.066 3.066 0 012.812-2.812zm7.44 5.252a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
        <div>
          <p class="text-gray-700 font-semibold dark:text-white">Perfume Landing Page</p>
          <p
            class="text-gray-500 text-sm md:text-base dark:text-d-text-secondary"
          >A sample perfume landing page for product display and marketing purpose.</p>
        </div>
      </div>
      <div class="absolute mx-auto h-48 w-48 bg-repeat top-8 -right-56 overflow-hidden dark:invisible">
        <div class="absolute left-0 top-0 w-72 h-72 bg-white transform translate-y-10 -translate-x-44 -rotate-45"></div>
        <div class="w-full h-full" :style='{"background-image":"url(" + require("./assets/svg/dots-teal.svg") +")"}'></div>
      </div>
    </div>
    
    <!-- GET TO KNOW ME -->
    <div class="mx-auto py-16 px-4 w-full max-w-screen-md relative font-open-sans">
      <p class="font-semibold text-2xl text-center text-gray-700 mb-8 md:text-2xl md:text-left dark:text-white">Get to know me</p>
      <div class="flex flex-col md:flex-row items-center">
        <img src="./assets/img/profile.jpg" class="rounded-full mb-8 w-1/4 md:w-1/6 md:mr-5 md:mb-0" />
        <p
          class="text-gray-600 text-xl md:text-xl dark:text-white"
        >I started web development since 2019 and I've been part of different software development projects both desktop and web application. 
        My eye for detail, creativity, and perfectionist nature have left me with many highly satisfied clients. 
       </p>
      </div>
      <div class="absolute mx-auto h-48 w-48 bg-repeat -bottom-2 -left-56 overflow-hidden transform rotate-180 dark:invisible">
        <div class="absolute left-0 top-0 w-72 h-72 bg-white transform translate-y-10 -translate-x-44 -rotate-45"></div>
        <div class="w-full h-full" :style='{"background-image":"url(" + require("./assets/svg/dots-teal.svg") +")"}'></div>
      </div>
    </div>
    <div class="pt-4 dark:text-white">
      <svg fill="currentColor" viewBox="0 0 1695 57" class="text-footer dark:text-d-tertiary">
        <path
          d="M0 23c135.4 19 289.6 28.5 462.5 28.5C721.9 51.5 936.7 1 1212.2 1c183.6-.1 344.5 7.3 482.8 22v34H0V23z"
        />
      </svg>
      <div class="bg-footer dark:bg-d-tertiary">
        <div class="mx-auto py-16 px-4 w-full max-w-screen-md">
          <p class="font-semibold text-gray-700 mb-8 text-2xl text-center md:text-3xl dark:text-white">Let's talk</p>
          <p class="text-xl font-light text-center">
           Wanna get in touch or talk about a project?
           <br>
            Feel free to contact me via email at <a href="mailto:keigofujita19@gmail.com" class="text-primary font-semibold">keigofujita19@gmail.com</a>
            or drop a line in the form at the 
            contact page
          </p>
        </div>
      </div>
    </div>
    <footer class="bg-primary dark:bg-d-footer">
      <div class="mx-auto py-8 px-4 w-full flex flex-col md:flex-row justify-between">
        <p class="text-white text-center mb-5 text-base md:text-sm md:mb-0 md:w-1/2">
          © Copyright 2021 Keigo Victor Fujita <span class="block md:inline"></span> All rights reserved.
        </p>
        <div class="flex justify-center items-center md:w-1/2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            class="w-6 h-6 text-white mx-2"
            viewBox="0 0 16 16"
          >
            <path
              d="M0 4a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V4zm2-1a1 1 0 0 0-1 1v.217l7 4.2 7-4.2V4a1 1 0 0 0-1-1H2zm13 2.383-4.758 2.855L15 11.114v-5.73zm-.034 6.878L9.271 8.82 8 9.583 6.728 8.82l-5.694 3.44A1 1 0 0 0 2 13h12a1 1 0 0 0 .966-.739zM1 11.114l4.758-2.876L1 5.383v5.73z"
            />
          </svg>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            class="w-6 h-6 text-white mx-2"
            viewBox="0 0 16 16"
          >
            <path
              d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"
            />
          </svg>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            class="w-6 h-6 text-white mx-2"
            viewBox="0 0 16 16"
          >
            <path
              d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"
            />
          </svg>
        </div>
      </div>
    </footer>
  </div>
  </div>
</template>

<script>
export default {
  created: function(){
    this.theme = localStorage.getItem('theme') || 'light';
  },
  data: function(){
    return{
      theme : 'light'
    }
  },
  name: 'Main',
  methods : {
     toggleDark : function() {
        this.theme = this.theme == 'light' ? 'dark' : 'light';
        localStorage.setItem('theme',this.theme)
     }
  }
}
</script>