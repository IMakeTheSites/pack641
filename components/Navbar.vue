<template>
  <nav class="relative flex flex-wrap items-center justify-between px-2 py-3 bg-blue-300 mb-3">
  <div class="container px-4 mx-auto flex flex-wrap items-center justify-between">
     <div class="w-full relative flex justify-between lg:w-auto  px-4 lg:static lg:block lg:justify-start">
        <NuxtLink to="/" class="flex items-center flex-no-shrink">
        <img src="~/assets/CubScoutLogo.svg" alt="Cub Scout Logo" title="Do your best!" />
        </NuxtLink>
        <button class="cursor-pointer text-xl leading-none px-3 py-1 border border-solid border-transparent rounded bg-transparent block lg:hidden outline-none focus:outline-none" type="button" v-on:click="toggleNavbar()">
<img src="~/assets/Hamburger_icon.svg" alt="hamburger" />
</button>
      </div>
      <div v-bind:class="{'hidden': !showMenu, 'flex': showMenu}" class="lg:flex lg:flex-grow items-center">
        <ul class="flex flex-col lg:flex-row list-none ml-auto">
            <li class="nav-item">
            <NuxtLink to="/" class="px-3 py-2 flex items-center text-xs uppercase font-bold leading-snug text-white hover:opacity-75">Home</NuxtLink>
            </li>
            <li class="nav-item">
            <NuxtLink to="/about" class="px-3 py-2 flex items-center text-xs uppercase font-bold leading-snug text-white hover:opacity-75">About</NuxtLink>
            </li>
            <li class="nav-item">
                <NuxtLink to="/contact" class="px-3 py-2 flex items-center text-xs uppercase font-bold leading-snug text-white hover:opacity-75">Contact</NuxtLink>
            </li>
            <li class="nav-item">
                <NuxtLink to="/user" class="px-3 py-2 flex items-center text-xs uppercase font-bold leading-snug text-white hover:opacity-75">User</NuxtLink>

            </li>
            <li class="nav-item">
                <a href="https://pack641.org/" class="px-3 py-2 flex items-center text-xs uppercase font-bold leading-snug text-white hover:opacity-75">Pack 641 Homepage</a>

            </li>
        </ul>
    </div>
  </div>
</nav>
</template>

<script>
export default {
    data() {
        return {
            showMenu: false
        }
    },
    methods: {
        toggleNavbar: function(){
            this.showMenu = !this.showMenu;
        }
    }

}
</script>

<style>

</style>