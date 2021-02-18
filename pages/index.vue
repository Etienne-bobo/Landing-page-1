<template>
  <div align="center">
    <nav
      class="top-0 absolute z-50 w-full flex flex-wrap items-center shadow-sm justify-between px-2 py-3 navbar-expand-lg"
    >
      <div
        class="container px-4 mx-auto flex flex-wrap items-center justify-between"
      >
        <div
          class="w-full relative flex justify-between lg:w-auto lg:static lg:block lg:justify-start"
        >
          <a
            class="text-xl font-bold leading-relaxed inline-block mr-4 py-2 whitespace-no-wrap uppercase text-gray-800"
            href="#"
            >NODIVO</a
          ><button
            class="cursor-pointer text-xl leading-none px-3 py-1 border border-solid border-transparent rounded bg-transparent block lg:hidden outline-none focus:outline-none"
            type="button"
            @click="toggleNavbar()"
          >
            <span class="material-icons text-6xl"> view_list </span>
          </button>
        </div>
        <div
          class="lg:flex flex-grow items-center bg-white lg:bg-transparent lg:shadow-none"
          :class="{ hidden: !showMenu, block: showMenu }"
        >
          <ul
            class="flex flex-col lg:flex-row mx-auto justify-center list-none mr-auto"
          >
            <li class="flex items-center">
              <a
                class="flex text-gray-800 rounded-md px-4 py-2 m-2 transition duration-500 ease select-none focus:outline-none focus:shadow-outline"
              >
                Comment ca marche?
              </a>
            </li>
            <li class="flex mx-auto items-center hidden lg:block mt-2">
              <div class="dropdown inline-block relative">
                <button
                  class="text-gray-800 py-2 px-4 rounded inline-flex items-center"
                >
                  <span class="mr-1">Platforme</span>
                  <svg
                    class="fill-current h-4 w-4"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 20 20"
                  >
                    <path
                      d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
                    />
                  </svg>
                </button>
                <ul class="dropdown-menu absolute hidden text-gray-700 pt-1">
                  <li class="">
                    <a
                      class="rounded-t bg-gray-200 text-gray-800 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                      href="#"
                      >Application web</a
                    >
                  </li>
                  <li class="">
                    <a
                      class="bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                      href="#"
                      >Application mobile</a
                    >
                  </li>
                </ul>
              </div>
            </li>
            <li class="flex items-center md:hidden">
              <a
                class="flex text-gray-800 rounded-md px-4 py-2 m-2 transition duration-500 ease select-none focus:outline-none focus:shadow-outline"
              >
                Application mobile
              </a>
            </li>
            <li class="flex items-center md:hidden">
              <a
                class="flex text-gray-800 rounded-md px-4 py-2 m-2 transition duration-500 ease select-none focus:outline-none focus:shadow-outline"
              >
                Application web
              </a>
            </li>
            <li class="flex items-center md:hidden">
              <a
                class="flex text-gray-800 rounded-md px-4 py-2 m-2 transition duration-500 ease select-none focus:outline-none focus:shadow-outline"
              >
                Help
              </a>
            </li>
            <li class="flex items-center">
              <a
                class="flex text-gray-800 rounded-md px-4 py-2 m-2 transition duration-500 ease select-none focus:outline-none focus:shadow-outline"
              >
                Nous Contacter
              </a>
            </li>
          </ul>

          <ul class="flex flex-col lg:flex-row list-none">
            <li class="flex items-center">
              <button
                class="flex items-center bg-blue-500 text-white active:bg-gray-100 text-xs font-bold uppercase px-4 py-2 rounded shadow hover:shadow-md outline-none focus:outline-none lg:mr-1 lg:mb-0 ml-3 mb-3"
                type="button"
                style="transition: all 0.15s ease 0s"
              >
                <span class="material-icons mr-2"> import_contacts </span> Blog
              </button>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <div class="mt-24 lg:mt-12 mx-auto">
      <div class="pb-12 max-w-7xl px-6 justify-center pt-32 md:mt-8 -mt-32">
        <h1
          class="lg:text-5xl text-gray-800 text-4xl font-bold flex justify-center"
        >
          Landing template for startups
        </h1>
        <p class="mt-8 mx-4 text-md text-gray-800 flex justify-center">
          Our landing page template works on all devices, so you only have to
          set it up once,
        </p>
        <div class="flex flex-wrap justify-center mt-8 mb-8">
          <div class="bg-green-500 rounded-md w-3/4 md:w-64 px-2 md:mr-4 mb-4">
            <div
              class="h-14 text-md text-white flex items-center justify-center"
            >
              <span class="material-icons mr-2 flex"> adb </span>Application
              mobile
            </div>
          </div>
          <div class="bg-blue-500 rounded-md w-3/4 md:w-64 px-2 mb-4">
            <div
              class="h-14 text-md text-white flex items-center justify-center"
            >
              <span class="material-icons mr-2 flex"> local_mall </span
              >Application web
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="max-w-6xl mx-4 mb-16">
      <img
        src="https://preview.cruip.com/open-pro/images/hero-image-01.jpg"
        alt=""
      />
    </div>
    <div class="mb-12">
      <h3 class="lg:text-5xl text-3xl text-gray-800 font-bold mb-6">
        Built exclusively for you
      </h3>
      <p class="text-xl">
        Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
        officia deserunt
      </p>
      <p class="text-xl">mollit laborum — semper quis lectus nulla.</p>
    </div>
    <div class="flex flex-wrap max-w-6xl">
      <div class="lg:pt-12 pt-8 w-full md:w-4/12 px-4 text-center">
        <div
          class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
        >
          <div class="px-4 py-5 flex-auto">
            <div
              class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-red-400"
            >
              <span class="material-icons text-white"> device_hub </span>
            </div>
            <h6 class="text-xl font-semibold">A Propos de nous</h6>
            <p class="mt-2 mb-4 text-gray-600">
              Divide details about your product or agency work into parts. A
              paragraph describing a feature will be enough.
            </p>
          </div>
        </div>
      </div>
      <div class="lg:pt-12 pt-8 w-full md:w-4/12 px-4 text-center">
        <div
          class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
        >
          <div class="px-4 py-5 flex-auto">
            <div
              class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-blue-500"
            >
              <span class="material-icons text-white"> stars </span>
            </div>
            <h6 class="text-xl font-semibold">A Propos de nous</h6>
            <p class="mt-2 mb-4 text-gray-600">
              Divide details about your product or agency work into parts. A
              paragraph describing a feature will be enough.
            </p>
          </div>
        </div>
      </div>
      <div class="lg:pt-12 pt-8 w-full md:w-4/12 px-4 text-center">
        <div
          class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
        >
          <div class="px-4 py-5 flex-auto">
            <div
              class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-green-500"
            >
              <span class="material-icons text-white"> verified_user </span>
            </div>
            <h6 class="text-xl font-semibold">A Propos de nous</h6>
            <p class="mt-2 mb-4 text-gray-600">
              Divide details about your product or agency work into parts. A
              paragraph describing a feature will be enough.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showMenu: false,
    }
  },
  methods: {
    toggleNavbar() {
      this.showMenu = !this.showMenu
    },
  },
}
</script>
<style scoped>
.dropdown:hover .dropdown-menu {
  display: block;
  width: 180px;
}
</style>
