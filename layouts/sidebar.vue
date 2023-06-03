<script setup>
  import { ref } from "vue";

  const isOpen = ref(false);
</script>

<template>
  <div>
    <div class="flex">
      <div
        :class="isOpen ? 'w-40' : 'w-60'"
        class="flex flex-col h-screen p-3 duration-300 bg-blue-800 shadow">
        <div class="space-y-3">
          <div class="flex items-center justify-between">
            <h2 class="text-xl font-bold text-white">Dashboard</h2>
            <button @click="isOpen = !isOpen">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6 text-white">
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
              </svg>
            </button>
          </div>
          <div class="relative">
            <span class="absolute inset-y-0 left-0 flex items-center py-4">
              <button type="submit" class="p-2 focus:outline-none focus:ring">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6">
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
                </svg>
              </button>
            </span>
            <input
              type="search"
              name="Search"
              placeholder="Search..."
              class="w-full py-2 pl-10 text-sm rounded-md focus:outline-none" />
          </div>
          <div class="flex-1">
            <ul class="pt-2 pb-4 space-y-1 text-sm">
              <li class="rounded-sm">
                <a href="#" class="flex items-center p-2 space-x-3 rounded-md">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100"
                    id="dashboard">
                    <path
                      d="M15.29,10.29l-2.78,2.78A2.09,2.09,0,0,0,12,13a2,2,0,0,0-2,2,2.09,2.09,0,0,0,.07.51l-.78.78a1,1,0,0,0,0,1.42,1,1,0,0,0,1.42,0l.78-.78A2.09,2.09,0,0,0,12,17a2,2,0,0,0,2-2,2.09,2.09,0,0,0-.07-.51l2.78-2.78a1,1,0,0,0-1.42-1.42ZM12,4A10,10,0,0,0,2,14a9.91,9.91,0,0,0,1.69,5.56,1,1,0,0,0,1.66-1.12,8,8,0,1,1,13.3,0,1,1,0,0,0,.27,1.39,1,1,0,0,0,.56.17,1,1,0,0,0,.83-.44A9.91,9.91,0,0,0,22,14,10,10,0,0,0,12,4Z"></path>
                  </svg>

                  <span>
                    <NuxtLink to="/admin/dashboard" class="text-gray-100"
                      >Dashboard</NuxtLink
                    >
                  </span>
                </a>
              </li>
              <li class="rounded-sm">
                <a href="#" class="flex items-center p-2 space-x-3 rounded-md">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100">
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
                  </svg>

                  <span>
                    <span>
                      <NuxtLink to="/admin/kelas" class="text-gray-100"
                        >Class</NuxtLink
                      >
                    </span>
                  </span>
                </a>
              </li>
              <li class="rounded-sm">
                <a href="#" class="flex items-center p-2 space-x-3 rounded-md">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    data-name="Layer 1"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100"
                    id="building">
                    <path
                      d="M14,8h1a1,1,0,0,0,0-2H14a1,1,0,0,0,0,2Zm0,4h1a1,1,0,0,0,0-2H14a1,1,0,0,0,0,2ZM9,8h1a1,1,0,0,0,0-2H9A1,1,0,0,0,9,8Zm0,4h1a1,1,0,0,0,0-2H9a1,1,0,0,0,0,2Zm12,8H20V3a1,1,0,0,0-1-1H5A1,1,0,0,0,4,3V20H3a1,1,0,0,0,0,2H21a1,1,0,0,0,0-2Zm-8,0H11V16h2Zm5,0H15V15a1,1,0,0,0-1-1H10a1,1,0,0,0-1,1v5H6V4H18Z"></path>
                  </svg>
                  <span>
                    <span>
                      <NuxtLink to="/admin/instansi" class="text-gray-100"
                        >Instansi</NuxtLink
                      >
                    </span>
                  </span>
                </a>
              </li>
              <li class="rounded-sm">
                <a href="#" class="flex items-center p-2 space-x-3 rounded-md">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100">
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M15.75 9V5.25A2.25 2.25 0 0013.5 3h-6a2.25 2.25 0 00-2.25 2.25v13.5A2.25 2.25 0 007.5 21h6a2.25 2.25 0 002.25-2.25V15M12 9l-3 3m0 0l3 3m-3-3h12.75" />
                  </svg>
                  <span class="text-gray-100"> Logout </span>
                </a>
              </li>
              <li class="rounded-sm">
                <a href="#" class="flex items-center p-2 space-x-3 rounded-md">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    data-name="Layer 2"
                    viewBox="0 0 48 48"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100"
                    id="graduate">
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M30.877 32.005a3.4 3.4 0 0 0-1.743-.355 3.072 3.072 0 0 0-.95.25l3.039 1.227a29.512 29.512 0 0 0-2.454 3.386A12.315 12.315 0 0 0 27.5 39.156a5.219 5.219 0 0 0-.321 2.324c1.45-.324 2.984-1.92 3.975-3.83a7.353 7.353 0 0 0 .978-4.018A2.218 2.218 0 0 0 30.877 32.005zM10.372 16.634v4.915L27.235 27.56h.01a33.269 33.269 0 0 0 3.861-.22c3.287-.48 5.416-1.4 5.416-2.368v-8.1L26.17 20.38z"></path>
                    <polygon
                      points="22.32 6.46 0 12.575 10.372 15.027 26.097 18.753 36.522 15.226 48 11.333 22.32 6.46"></polygon>
                    <path
                      d="M25.7,39.768c.021-.1.042-.219.062-.344s.063-.271.115-.417l.032-.094A15.359,15.359,0,0,1,27.433,35.7a16.88,16.88,0,0,1,1.252-1.826.419.419,0,0,0,.042-.063l-2.056-.824a7.6,7.6,0,0,0-1.221,1.7,13.808,13.808,0,0,0-1.114,2.423L.532,26.5l-.146.637c-.2.981-.146,2.024.491,2.285L25.983,41.375C25.638,41.114,25.555,40.54,25.7,39.768Z"></path>
                    <polygon
                      points=".045 24.569 .047 24.565 .041 24.562 .045 24.569"></polygon>
                    <path
                      d="M24.058 33.967c1.418-2.731 3.907-4.3 5.823-3.791l-.075-.028L3.581 20.786c-.975-.415-2.372.689-3.141 2.5a6.193 6.193 0 0 0-.393 1.28L23.579 35.052A9.347 9.347 0 0 1 24.058 33.967zM45.256 17.646V13.921l-1.566.522v3.2a1.881 1.881 0 0 0-1.116 1.722v1.325a1.894 1.894 0 1 0 3.788 0V19.368A1.872 1.872 0 0 0 45.256 17.646z"></path>
                  </svg>
                  <span class="text-gray-100"> Profession </span>
                </a>
              </li>
              <li class="rounded-sm">
                <a href="#" class="flex items-center p-2 space-x-3 rounded-md">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100"
                    id="account">
                    <path
                      d="M15.71,12.71a6,6,0,1,0-7.42,0,10,10,0,0,0-6.22,8.18,1,1,0,0,0,2,.22,8,8,0,0,1,15.9,0,1,1,0,0,0,1,.89h.11a1,1,0,0,0,.88-1.1A10,10,0,0,0,15.71,12.71ZM12,12a4,4,0,1,1,4-4A4,4,0,0,1,12,12Z"></path>
                  </svg>
                  <span class="text-gray-100"> Kelola akun </span>
                </a>
              </li>
              <li class="rounded-sm">
                <a href="#" class="flex items-center p-2 space-x-3 rounded-md"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    width="40"
                    height="40"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100"
                    id="book">
                    <path
                      d="M43.3 39.6c-.6 2.5-3.7 1.1-2.4 1.4l-19.7-5c-1.1-.3-1.7-1.4-1.4-2.4.3-1.1 1.4-1.7 2.4-1.4l19.7 5.1c1 .2 1.6 1.3 1.4 2.3zm-1.5 11-19.7-5.1c-1.1-.3-2.2.4-2.4 1.4-.3 1.1.4 2.2 1.4 2.4l19.7 5.1c-1.3-.3 1.8.9 2.4-1.4.3-1-.3-2.1-1.4-2.4zm-5.9 11.7-13.8-3.6c-1.1-.3-2.2.4-2.4 1.4-.3 1.1.4 2.2 1.4 2.4l13.8 3.6c-1.3-.3 1.8.9 2.4-1.4.3-1-.3-2.1-1.4-2.4zM90 19v52.5c0 .9-.6 1.7-1.5 1.9l-38 9.5c-.3.1-.7.1-1 0l-38-9.5c-.9-.2-1.5-1-1.5-1.9V19c0-1.3 1.2-2.3 2.5-1.9L50 26.5l37.5-9.4c1.3-.4 2.5.6 2.5 1.9zM48 30.1l-34-8.5v48.3l34 8.5V30.1zm38-8.5-34 8.5v48.3l34-8.5V21.6zm-5.8 12c-.3-1.1-1.4-1.7-2.4-1.4l-19.7 5.1c-1.1.3-1.7 1.4-1.4 2.4.6 2.5 3.7 1.1 2.4 1.4L78.8 36c1.1-.3 1.7-1.4 1.4-2.4zm0 13.4c-.3-1.1-1.4-1.7-2.4-1.4l-19.7 5.1c-1.1.3-1.7 1.4-1.4 2.4.6 2.4 3.7 1.1 2.4 1.4l19.7-5.1c1.1-.3 1.7-1.4 1.4-2.4zm-5.9 14.7c-.3-1.1-1.4-1.7-2.4-1.4l-13.8 3.6c-1.1.3-1.7 1.4-1.4 2.4.6 2.5 3.7 1.1 2.4 1.4l13.8-3.5c1.1-.3 1.7-1.4 1.4-2.5z"></path>
                    <path
                      fill="#00F"
                      d="M1644-930V754H-140V-930h1784m8-8H-148V762h1800V-938z"></path>
                  </svg>
                  <span class="text-gray-100">E-Books</span>
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="container mx-auto mt-12">
        <slot />
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped></style>

<!-- <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 text-gray-100">
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M9.594 3.94c.09-.542.56-.94 1.11-.94h2.593c.55 0 1.02.398 1.11.94l.213 1.281c.063.374.313.686.645.87.074.04.147.083.22.127.324.196.72.257 1.075.124l1.217-.456a1.125 1.125 0 011.37.49l1.296 2.247a1.125 1.125 0 01-.26 1.431l-1.003.827c-.293.24-.438.613-.431.992a6.759 6.759 0 010 .255c-.007.378.138.75.43.99l1.005.828c.424.35.534.954.26 1.43l-1.298 2.247a1.125 1.125 0 01-1.369.491l-1.217-.456c-.355-.133-.75-.072-1.076.124a6.57 6.57 0 01-.22.128c-.331.183-.581.495-.644.869l-.213 1.28c-.09.543-.56.941-1.11.941h-2.594c-.55 0-1.02-.398-1.11-.94l-.213-1.281c-.062-.374-.312-.686-.644-.87a6.52 6.52 0 01-.22-.127c-.325-.196-.72-.257-1.076-.124l-1.217.456a1.125 1.125 0 01-1.369-.49l-1.297-2.247a1.125 1.125 0 01.26-1.431l1.004-.827c.292-.24.437-.613.43-.992a6.932 6.932 0 010-.255c.007-.378-.138-.75-.43-.99l-1.004-.828a1.125 1.125 0 01-.26-1.43l1.297-2.247a1.125 1.125 0 011.37-.491l1.216.456c.356.133.751.072 1.076-.124.072-.044.146-.087.22-.128.332-.183.582-.495.644-.869l.214-1.281z" />
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                  </svg> -->
