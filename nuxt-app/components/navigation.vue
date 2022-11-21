<!-- Code for Navigation Route -->
<template>
    <div class=" box-border shadow">
      <nav class="flex">
        <ul
          class="
            inline-flex
            flex-col
            text-center
            pt-5
            shadow-2xl
            bg-slate-100
            nav
          "
        >
          <div class="w-48 text-center">
            <li class="pt-6">
              <!-- defining nuxt links us -->
              <NuxtLink class="active:text-blue-200 hover:text-blue-700" to="/"
                >Home</NuxtLink
              >
            </li>
            <li class="pt-6">
              <NuxtLink class="active:text-blue-200 hover:text-blue-700" to="/data">Dashboard</NuxtLink>
            </li>
            <li class="pt-6">
              <NuxtLink class="active:text-blue-200 hover:text-blue-700" to="/note/">Note</NuxtLink>
            </li>
          </div>
        </ul>
  <ul class=" w-full text-center">
        <NuxtPage class="p-5 text-center" />
  </ul>
      </nav>
    </div>
  </template>