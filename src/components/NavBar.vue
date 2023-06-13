<template>
  <header class="p-5 bg-neutral-50 text-slate-700 dark:bg-gray-900 dark:text-gray-100">
    <nav class="container flex justify-between h-10 mx-auto">
      <a
        rel="noopener noreferrer"
        href="/"
        aria-label="Back to homepage"
        class="flex items-center p-2"
      >
        <img
          src="../assets/logoAchilleus.png"
          alt="logo Achilleus"
          width="40"
          height="40"
          class="d-inline-block"
        />
        <p class="px-2 font-bold dark:text-gray-200">
          <router-link to="/">Achilleus Trading Bot</router-link>
        </p>
      </a>
      <ul id="menu" class="items-stretch space-x-3 md:flex" :class="classMenu">
        <li class="flex">
          <a
            rel="noopener noreferrer"
            class="flex items-center px-4 -mb-1 hover:border-b-2 dark:text-gray-100"
            ><router-link to="/">Présentation</router-link></a
          >
        </li>
        <li class="flex">
          <a
            rel="noopener noreferrer"
            href="#"
            class="flex items-center px-4 -mb-1 hover:border-b-2 dark:text-gray-100"
            ><router-link to="/demo">Démo</router-link></a
          >
        </li>
        <li class="flex">
          <a
            rel="noopener noreferrer"
            href="#"
            class="flex items-center px-4 -mb-1 hover:border-b-2 dark:text-gray-100"
            ><router-link to="/faq">F.A.Q.</router-link></a
          >
        </li>
        <li class="flex">
          <a
            rel="noopener noreferrer"
            href="#"
            class="flex items-center px-4 -mb-1 hover:border-b-2 dark:text-gray-100"
            ><router-link to="/contact">Contact</router-link></a
          >
        </li>
        <li class="flex">
          <a
            rel="noopener noreferrer"
            href="#"
            class="flex items-center px-4 -mb-1 dark:text-gray-100"
          >
            <img
              src="../assets/telegram.png"
              alt="logo telegram"
              width="30"
              height="30"
              class="d-inline-block"
            />
          </a>
        </li>
      </ul>
      <button class="flex justify-end p-4 md:hidden" @click="toggleMenu">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          class="w-6 h-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16M4 18h16"
          ></path>
        </svg>
      </button>
    </nav>
  </header>
</template>

<script>
export default {
  data(){
    return {
      menuVisible: true
    }
  },
  computed: {
    classMenu(){
        if(this.menuVisible){
          return {hidden: true};
        } else {
          return {hidden: false, "absolute flex leading-[3] bg-[lightgray] h-[64vh] flex-col mt-[70px] right-0;":true};
        }
      }
  },
  methods: {
    toggleMenu() {
      this.menuVisible = !this.menuVisible
    }
  }
};
</script>
