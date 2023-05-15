<template>
  <nav
    class="px-6 sm:px-20 py-2.5 dark:bg-gray-900 fixed w-full z-20 top-0 left-0 lg:px-2"
  >
    <div class="container flex flex-wrap justify-between items-center mx-auto">
      <a href="https://flowbite.com/" class="flex items-center">
        <img
          src="../assets/img/terapi.png"
          class="mr-3 h-[4rem] w-[4rem] sm:h-[4rem]"
          alt="Flowbite Logo"
        />
        <span class="self-center text-xl font-semibold whitespace-nowrap text-white"
          >Hypnotherapy
        </span>
      </a>
      <div class="flex md:order-2">
        <ul
          class="hidden md:flex items-center p-4 mt-4 md:flex-row md:mt-0 md:text-sm md:font-medium md:border-0"
        >
          <li>
            <a
              href="#"
              class="block py-2 pr-4 pl-3 text-[16px] font-bold text-white"
              aria-current="page"
              >Beranda</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pr-4 pl-3 text-[16px] font-bold text-white"
              aria-current="page"
              >Hipnoterapi</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pr-4 pl-3 text-[16px] font-bold text-white"
              aria-current="page"
              >FAQ</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pr-4 pl-3 text-[16px] font-bold text-white"
              aria-current="page"
              >Profil</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pr-4 pl-3 text-[16px] font-bold text-white"
              aria-current="page"
              >Forms</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pr-4 pl-3 text-[16px] font-bold text-white"
              aria-current="page"
              >Galeri</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pr-4 pl-3 text-[16px] font-bold text-center text-gray-900 bg-white border border-gray-200 rounded-full focus:outline-none hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700"
              >Kontak</a
            >
          </li>
        </ul>
        <div class="md:hidden lg:hidden">
          <svg
            class="w-6 h-6 text-white"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
            @click="isOpen = true"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            ></path>
          </svg>
        </div>
      </div>
    </div>
  </nav>

  <!-- Drawer Menu Mobile -->
  <div
    v-show="isOpen"
    @click="isOpen = false"
    @mouseleave="isOpen = false"
    id="drawer-navigation"
    class="fixed z-40 p-4 overflow-y-auto bg-white w-full dark:bg-gray-800 rounded-md"
    tabindex="-1"
    aria-labelledby="drawer-navigation-label"
  >
    <div class="p-4 flex justify-between items-center">
      <h5
        id="drawer-navigation-label"
        class="text-base font-semibold text-gray-500 uppercase dark:text-gray-400"
      >
        Menu
      </h5>
      <button
        type="button"
        data-drawer-dismiss="drawer-navigation"
        aria-controls="drawer-navigation"
        class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm inline-flex items-center dark:hover:bg-gray-600 dark:hover:text-white"
      >
        <svg
          aria-hidden="true"
          class="w-5 h-5"
          fill="currentColor"
          viewBox="0 0 20 20"
          xmlns="http://www.w3.org/2000/svg"
          @click="close"
        >
          <path
            fill-rule="evenodd"
            d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
            clip-rule="evenodd"
          ></path>
        </svg>
        <span class="sr-only">Close menu</span>
      </button>
    </div>

    <div class="py-2 overflow-y-auto">
      <ul class="space-y-2">
        <li>
          <a
            href="#"
            class="flex items-center p-4 text-base font-normal text-gray-900 rounded-lg hover:bg-gray-100"
          >
            <span class="">Beranda</span>
          </a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center p-4 text-base font-normal text-gray-900 rounded-lg hover:bg-gray-100"
          >
            <span class="">Hipnoterapi</span>
          </a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center p-4 text-base font-normal text-gray-900 rounded-lg hover:bg-gray-100"
          >
            <span class="">FAQ</span>
          </a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center p-4 text-base font-normal text-gray-900 rounded-lg hover:bg-gray-100"
          >
            <span class="">Profil</span>
          </a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center p-4 text-base font-normal text-gray-900 rounded-lg hover:bg-gray-100"
          >
            <span class="">Forms</span>
          </a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center p-4 text-base font-normal text-gray-900 rounded-lg hover:bg-gray-100"
          >
            <span class="">Galeri</span>
          </a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center p-4 text-base font-normal text-gray-900 rounded-lg hover:bg-gray-100"
          >
            <span class="">Kontak</span>
          </a>
        </li>
      </ul>
    </div>
  </div>
  <!-- End Drawer Menu Mobile -->
</template>

<script>
export default {
  name: "HomeView",
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    close() {
      this.isOpen = false;
    },
  },
};
</script>
