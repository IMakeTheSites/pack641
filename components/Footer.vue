<template>
  <footer id="Footer" class=" h-auto content-start items-start w-full z-9 font-body fixed bottom-0 bg-gray-700 text-gray-200 flex flex-col">
      <div class="h-auto content-start flex mx-auto items-start px-2 pt-3 pb-3 md:p-6 mb-8 flex-col md:flex-row max-w-7xl">
			<div class="h-auto flex flex-row mx-2 md:mx-0">
				<NuxtLink :prefetch="false" to="/" class="p-2 my-4 mx-0 flex">
                        <img src="~/assets/CubScoutLogo.svg" alt="Cub Scout Logo" title="Do your best!" />
                </NuxtLink>
            </div>
            			<div class="flex flex-col">
              <span class="flex flex-row m-4 mx-auto flex-wrap">
                  <ul>
                      <li><NuxtLink to="/" class="w-6 mx-2 md:mx-4 text-gray-400 hover:text-white">Home</NuxtLink></li>
                      <li><NuxtLink to="/about" class="w-6 mx-2 md:mx-4 text-gray-400 hover:text-white">About</NuxtLink></li>
<li><NuxtLink to="/user" class=" w-6 mx-2 md:mx-4 text-gray-400 hover:text-white">User</NuxtLink></li>
<li><NuxtLink to="/contact" class=" w-6 mx-2 md:mx-4 text-gray-400 hover:text-white">Contact</NuxtLink></li>
<li><a href="https://pack641.org/" class=" w-6 mx-2 md:mx-4 text-gray-400 hover:text-white">Pack 641 Homepage</a></li>
                  </ul>
              </span></div></div>

  </footer>
</template>

<script>
export default {

}
</script>

<style>

</style>