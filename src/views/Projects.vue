<template>
  <div>
    <!-- LANDING PAGE -->
    <div class="mx-auto py-24 px-2 w-full max-w-screen-lg font-open-sans">
      <div class="flex flex-col-reverse md:flex-row justify-between">
        <div class="text-center md:text-left">
          <h1
            class="text-4xl md:text-6xl font-bold md:font-semibold text-gray-800 mb-2 md:mb-2 dark:text-white"
          >My Projects</h1>
          <div class="mx-auto pt-4 px-8 md:px-1 w-full max-w-screen-lg font-open-sans">
            <p
              class="text-xl md:text-3xl text-gray-500 dark:text-white"
            >I’ve designed and developed different websites and desktop applications for the past two years. Below are some of my favorites.</p>
          </div>
        </div>
        <img src="@/assets/svg/projects.svg" alt srcset class="mx-auto w-96 mb-16 md:mb-0" />
      </div>
    </div>

    <div class=" dark:bg-d-footer content-wrapper font-open-sans">
      <div class="max-w-screen-xl mx-auto px-8">
        <!-- PROJECT 1 -->
        <div class="flex flex-col md:flex-row py-24">
          <!-- IMAGE -->
          <div class="w-full md:w-1/2">
            <div class="relative img-holder mb-12 md:mb-0" style="z-index: 1;">
              <div
                class="img-under bg-l-project-overlay w-full h-full absolute -top-4 -left-4 rounded"
                style="z-index: -1;"
              ></div>
              <div class="project-image relative top-0 left-0">
                <img
                  src="/img/projects/project1.PNG"
                  alt="Sunpack ERP"
                  class="w-full rounded"
                  style="z-index: 2;"
                />
              </div>
            </div>
          </div>
          <!-- TEXT AND BUTTON-->
          <div class="px-0 md:px-8 w-full md:w-1/2">
            <h1 class="text-4xl font-semibold text-gray-700 dark:text-white mb-5">Sunpack ERP</h1>
            <p
              class="text-gray-600 dark:text-gray-200 text-xl mb-12"
            >An Enterprise Resource Planning software for a carton manufacturing company. Sunpack ERP integrates all software and business processes on a single system. Built with Powerbuilder and SQL Server.</p>
            <button
              class="bg-primary dark:bg-d-secondary text-white w-32 px-4 py-2 shadow-lg rounded text-sm focus:outline-none focus:ring-2 focus:ring-blue-300 ring-offset-2 focus:ring-offset-blue-200"
            >View More</button>
          </div>
        </div>

        <!-- PROJECT 2 -->
        <div class="flex flex-col-reverse md:flex-row py-12">
          <!-- TEXT AND BUTTON-->
          <div class="px-0 md:px-8 w-full md:w-1/2">
            <h1 class="text-4xl font-semibold text-gray-700 dark:text-white mb-5">Gardner College Clearance System</h1>
            <p
              class="text-gray-600 dark:text-gray-200 text-xl mb-12"
            >An efficient and computerized clearance system (web-based application) for the school. Gardner College Clearance System is capable of handling comprehensive information of the student in a simultaneous and speedy way.</p>
            <a
              href="https://gardner-college.tk"
              target="_blank"
              class="text-decoration-none bg-primary dark:bg-d-secondary text-white w-32 px-8 py-2 shadow-lg rounded text-sm focus:outline-none focus:ring-2 focus:ring-blue-300 ring-offset-2 focus:ring-offset-blue-200"
            >View More</a>
          </div>

          <!-- IMAGE -->
          <div class="w-full md:w-1/2 mb-12 md:mb-0" style="z-index: 1;">
            <div class="relative img-holder" style="z-index: 1;">
              <div
                class="img-under bg-l-project-overlay w-full h-full absolute -top-4 -left-4 rounded"
                style="z-index: -1;"
              ></div>
              <div class="project-image relative top-0 left-0">
                <img
                  src="/img/projects/project2.PNG"
                  alt="Sunpack ERP"
                  class="w-full rounded"
                  style="z-index: 2;"
                />
              </div>
            </div>
          </div>
        </div>

        <!-- PROJECT 3 -->
        <div class="flex flex-col md:flex-row py-24">
          <!-- IMAGE -->
          <div class="w-full md:w-1/2 mb-12 md:mb-0">
            <div class="relative img-holder" style="z-index: 1;">
              <div
                class="img-under bg-l-project-overlay w-full h-full absolute -top-4 -left-4 rounded"
                style="z-index: -1;"
              ></div>
              <div class="project-image relative top-0 left-0">
                <img
                  src="/img/projects/project3.PNG"
                  alt="Sunpack ERP"
                  class="w-full rounded"
                  style="z-index: 2;"
                />
              </div>
            </div>
          </div>
          <!-- TEXT AND BUTTON-->
          <div class="px-0 md:px-8 w-full md:w-1/2">
            <h1 class="text-4xl font-semibold text-gray-700 dark:text-white mb-5">Perfume Landing page</h1>
            <p
              class="text-gray-600 dark:text-white text-xl mb-12"
            >A sample perfume landing page for product display and marketing purpose.</p>
            <a
              href="https://codewithkeigo-perfume.netlify.com"
              target="_blank"
              class="text-decoration-none bg-primary dark:bg-d-secondary text-white w-32 px-8 py-2 shadow-lg rounded text-sm focus:outline-none focus:ring-2 focus:ring-blue-300 ring-offset-2 focus:ring-offset-blue-200"
            >View More</a>
          </div>
        </div>
      </div>
    </div>

    <div class="pt-4 dark:text-white dark:bg-d-footer">
      <svg fill="currentColor" viewBox="0 0 1695 57" class="text-footer dark:text-d-tertiary">
        <path
          d="M0 23c135.4 19 289.6 28.5 462.5 28.5C721.9 51.5 936.7 1 1212.2 1c183.6-.1 344.5 7.3 482.8 22v34H0V23z"
        />
      </svg>
      <div class="bg-footer dark:bg-d-tertiary">
        <div class="mx-auto py-16 px-4 w-full max-w-screen-lg">
          <p
            class="font-semibold text-gray-700 mb-8 text-2xl text-center md:text-3xl dark:text-white"
          >Let's talk</p>
          <p class="text-xl font-light text-center">
            Wanna get in touch or talk about a project?
            <br />Feel free to contact me via email at
            <a
              href="mailto:keigofujita19@gmail.com"
              class="text-primary font-semibold"
            >keigofujita19@gmail.com</a>
            or drop a line in the form at the
            contact page
          </p>
        </div>
      </div>
    </div>
    <footer class="bg-primary dark:bg-d-footer">
      <div class="mx-auto py-8 px-4 w-full flex flex-col md:flex-row justify-between">
        <p class="text-white text-center mb-5 text-base md:text-sm md:mb-0 md:w-1/2">
          © Copyright 2021 Keigo Victor Fujita
          <span class="block md:inline"></span> All rights reserved.
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
</template>

<script>
export default {
 
}
</script>
