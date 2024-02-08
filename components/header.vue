<template>
  <nav
    class="flex flex-wrap w-full h-20 m-auto p-2 text-white md:justify-between justify-center items-center z-10"
  >
    <!--Image of the W school logo from public directory if click return to home page-->
    <nuxt-link to="/">
      <div className="text-3xl text-semibold">Winter School</div>
    </nuxt-link>
    <!--Navigation bar-->
    <navigationMenu class="hidden md:block w-1/2" />
  </nav>
</template>

<script>
import navigationMenu from "./navigation-menu.vue";
export default {
  components: {
    navigationMenu,
  },
};
</script>
