<template>
  <div>
    <div class="py-24">
      <h1
        class="text-2xl md:text-4xl text-center font-semibold font-open-sans text-primary dark:text-white"
      >
        GET IN TOUCH NOW!
      </h1>
      <div
        class="mx-auto pt-8 md:pt-16 px-8 md:px-2 w-full max-w-screen-lg font-open-sans"
      >
        <div class="flex flex-col md:flex-row justify-between md:space-x-12">
          <img
            src="@/assets/svg/contact.svg"
            alt
            srcset
            class="mt-12 mx-auto w-5/6 md:w-1/2 h-1/2 mb-16 md:mb-0"
          />
          <div class="w-full md:w-1/2">
            <form
              name="contact"
              method="post"
              data-netlify="true"
              data-netlify-honeypot="bot-field"
              enctype="application/x-www-form-urlencoded"
              @submit.prevent="handleFormSubmit"
            >
              <div class="mb-4">
                <p for class="text-primary dark:text-white mb-2">Name*</p>
                <input
                  v-model="form.name"
                  type="text"
                  name="name"
                  class="text-lg dark:bg-blue-100 px-4 py-1 w-full h-12 bg-gray-100 rounded border-2 border-primary focus:outline-none"
                />
              </div>

              <div class="mb-4">
                <p for class="text-primary dark:text-white mb-2">Email*</p>
                <input
                  v-model="form.email"
                  type="email"
                  name="email"
                  class="text-lg dark:bg-blue-100 px-4 py-1 w-full h-12 bg-gray-100 rounded border-2 border-primary focus:outline-none"
                />
              </div>

              <div class="mb-4">
                <p for class="text-primary dark:text-white mb-2">Subject*</p>
                <input
                  v-model="form.subject"
                  type="text"
                  name="subject"
                  class="text-lg dark:bg-blue-100 px-4 py-1 w-full h-12 bg-gray-100 rounded border-2 border-primary focus:outline-none"
                />
              </div>

              <div class="mb-4">
                <p for class="text-primary dark:text-white mb-2">Message*</p>
                <textarea
                  v-model="form.message"
                  name="message"
                  id=""
                  cols="30"
                  rows="30"
                  class="text-lg dark:bg-blue-100 px-4 py-1 w-full h-36 bg-gray-100 rounded border-2 border-primary focus:outline-none"
                ></textarea>
              </div>

              <button
                type="submit"
                class="px-8 py-2 bg-primary dark:bg-d-secondary text-white text-base rounded focus:outline-none"
              >
                Send Message
              </button>
            </form>
          </div>
        </div>
      </div>
    </div>

    <footer class="bg-primary dark:bg-d-footer">
      <div
        class="mx-auto py-8 px-4 w-full flex flex-col md:flex-row justify-between"
      >
        <p
          class="text-white text-center mb-5 text-base md:text-sm md:mb-0 md:w-1/2"
        >
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
import axios from "axios";
export default {
  data: function(){    
    return {
      form : {
        name : '',
        email: '',
        subject: '',
        message: ''
     }
    }
  },
  methods: {
    encode(data) {  
            const formData = new FormData();
            
            for (const key of Object.keys(data)) {
                formData.append(key, data[key]);
            }
            
            return formData;
        },

    handleFormSubmit(e) {
        const axiosConfig = {
            header: { "Content-Type": "application/x-www-form-urlencoded" }
        };

        axios.post(
            location.href, 
            this.encode({
                'form-name': e.target.getAttribute("name"),
                ...this.form,
            }),
            axiosConfig
        )
        .then(data => console.log(data))
        .catch(error => console.log(error))
        .then(console.log('Success'))
    }
  }
}
</script>