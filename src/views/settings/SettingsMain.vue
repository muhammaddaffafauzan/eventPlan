<template>
<!-- component -->
<div v-if="!isClosed" key="open" class="w-10/12 mx-auto max-w-6xl">
    <button @click="closePage" class="absolute top-4 left-4 focus:outline-none">
        <svg
          class="h-6 w-6 text-gray-600 hover:text-indigo-600 transition duration-300"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          aria-hidden="true"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M6 18L18 6M6 6l12 12"
          />
        </svg>
      </button>
<div class="lg:col-start-2 col-span-12 lg:col-span-10 grid grid-cols-6 gap-x-8 gap-y-10 border-b border-gray-900/10 pb-12 mx-auto">
  <div class="p-4 col-span-6 md:col-span-2 ">
      <div class="grid grid-cols-5">
        <div class="md:col-span-5 group relative flex items-left gap-x-6 rounded-lg p-3 text-sm leading-6 hover:bg-indigo-50 ">
          <div style="text-align: center;" class="flex h-11 w-11 flex-none items-center justify-center rounded-lg bg-gray-50 group-hover:bg-white mx-auto md:mx-0">
            <svg class="mx-auto items-center justify-center h-6 w-6 text-gray-600 group-hover:text-indigo-600" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M10.5 6a7.5 7.5 0 107.5 7.5h-7.5V6z" />
              <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 10.5H21A7.5 7.5 0 0013.5 3v7.5z" />
            </svg>
          </div>
          <div class="flex-auto hidden md:block">
            <a href="#" class="block font-semibold text-gray-900">
              Personal Information
              <span class="absolute inset-0"></span>
            </a>
            <p class="mt-1 text-gray-600">Get a better understanding of your traffic</p>
          </div>
        </div>
        <div class="md:col-span-5 group relative flex items-left justify-left gap-x-6 rounded-lg p-3 text-sm leading-6 hover:bg-gray-50">
          <div class="flex h-11 w-11 flex-none items-center justify-center rounded-lg bg-gray-50 group-hover:bg-white  mx-auto md:mx-0">
            <svg class="h-6 w-6 text-gray-600 group-hover:text-indigo-600" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M15.042 21.672L13.684 16.6m0 0l-2.51 2.225.569-9.47 5.227 7.917-3.286-.672zM12 2.25V4.5m5.834.166l-1.591 1.591M20.25 10.5H18M7.757 14.743l-1.59 1.59M6 10.5H3.75m4.007-4.243l-1.59-1.59" />
            </svg>
          </div>
          <div class="flex-auto  hidden md:block">
            <a href="#" class="block font-semibold text-gray-900">
              Engagement
              <span class="absolute inset-0"></span>
            </a>
            <p class="mt-1 text-gray-600">Speak directly to your customers</p>
          </div>
        </div>
        <div class="md:col-span-5 group relative flex items-center gap-x-6 rounded-lg p-3 text-sm leading-6 hover:bg-gray-50">
          <div class="flex h-11 w-11 flex-none items-center justify-center rounded-lg bg-gray-50 group-hover:bg-white  mx-auto md:mx-0">
            <svg class="h-6 w-6 text-gray-600 group-hover:text-indigo-600" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M7.864 4.243A7.5 7.5 0 0119.5 10.5c0 2.92-.556 5.709-1.568 8.268M5.742 6.364A7.465 7.465 0 004.5 10.5a7.464 7.464 0 01-1.15 3.993m1.989 3.559A11.209 11.209 0 008.25 10.5a3.75 3.75 0 117.5 0c0 .527-.021 1.049-.064 1.565M12 10.5a14.94 14.94 0 01-3.6 9.75m6.633-4.596a18.666 18.666 0 01-2.485 5.33" />
            </svg>
          </div>
          <div class="flex-auto  hidden md:block">
            <a href="#" class="block font-semibold text-gray-900">
              Security
              <span class="absolute inset-0"></span>
            </a>
            <p class="mt-1 text-gray-600">Your customers’ data will be safe and secure</p>
          </div>
        </div>
        <div class="md:col-span-5 group relative flex items-center gap-x-6 rounded-lg p-3 text-sm leading-6 hover:bg-gray-50">
          <div class="flex h-11 w-11 flex-none items-center justify-center rounded-lg bg-gray-50 group-hover:bg-white  mx-auto md:mx-0">
            <svg class="h-6 w-6 text-gray-600 group-hover:text-indigo-600" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 16.875h3.375m0 0h3.375m-3.375 0V13.5m0 3.375v3.375M6 10.5h2.25a2.25 2.25 0 002.25-2.25V6a2.25 2.25 0 00-2.25-2.25H6A2.25 2.25 0 003.75 6v2.25A2.25 2.25 0 006 10.5zm0 9.75h2.25A2.25 2.25 0 0010.5 18v-2.25a2.25 2.25 0 00-2.25-2.25H6a2.25 2.25 0 00-2.25 2.25V18A2.25 2.25 0 006 20.25zm9.75-9.75H18a2.25 2.25 0 002.25-2.25V6A2.25 2.25 0 0018 3.75h-2.25A2.25 2.25 0 0013.5 6v2.25a2.25 2.25 0 002.25 2.25z" />
            </svg>
          </div>
          <div class="flex-auto  hidden md:block">
            <a href="#" class="block font-semibold text-gray-900">
              Integrations
              <span class="absolute inset-0"></span>
            </a>
            <p class="mt-1 text-gray-600">Connect with third-party tools</p>
          </div>
        </div>
        <div class="md:col-span-5 group relative flex items-center gap-x-6 rounded-lg p-3 text-sm leading-6 hover:bg-gray-50">
          <div class="flex h-11 w-11 flex-none items-center justify-center rounded-lg bg-gray-50 group-hover:bg-white  mx-auto md:mx-0">
            <svg class="h-6 w-6 text-gray-600 group-hover:text-indigo-600" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M16.023 9.348h4.992v-.001M2.985 19.644v-4.992m0 0h4.992m-4.993 0l3.181 3.183a8.25 8.25 0 0013.803-3.7M4.031 9.865a8.25 8.25 0 0113.803-3.7l3.181 3.182m0-4.991v4.99" />
            </svg>
          </div>
          <div class="flex-auto  hidden md:block">
            <a href="#" class="block font-semibold text-gray-900">
              Automations
              <span class="absolute inset-0"></span>
            </a>
            <p class="mt-1 text-gray-600">Build strategic funnels that will convert</p>
          </div>
        </div>
      </div>
  </div>
  <div class="p-4 col-span-6 md:col-span-4">
    <router-view></router-view>
  </div>
</div>
</div>
</template>
<script>
export default {
  data() {
    return {
      isClosed: false,
    };
  },
  methods: {
    closePage() {
      this.isClosed = true;
      // Menambahkan delay untuk memberi waktu pada animasi fade
      setTimeout(() => {
        // Reset isClosed setelah animasi selesai
        this.isClosed = false;
      }, 500);
      // Simpan URL halaman terakhir di localStorage
      localStorage.setItem('lastVisitedPage', this.$route.fullPath);
      // Kembali ke halaman sebelumnya
      this.$router.go(-1);
    },
  },
  mounted() {
    // Periksa apakah ada URL halaman terakhir yang disimpan di localStorage
    const lastVisitedPage = localStorage.getItem('lastVisitedPage');
    // Jika ada, arahkan pengguna ke halaman terakhir yang disimpan
    if (lastVisitedPage) {
      this.$router.push(lastVisitedPage);
      // Hapus URL halaman terakhir dari localStorage setelah mengarahkan ke halaman tersebut
      localStorage.removeItem('lastVisitedPage');
    }
  }
};

</script>

<style>
/* Add this style block to your component's style block */
.fade-enter-active, .fade-leave-active {
    transition: opacity 0.5s ease-out; /* Adjust the transition duration and easing function as needed */
  }
  .fade-enter, .fade-leave-to {
    opacity: 0;
    transition-delay: 0.3s; /* Adjust the delay duration as needed */
  }
  
  /* Additional styling for smoother transition */
  .router-view-container {
    position: relative;
    overflow: hidden;
  }
</style>
