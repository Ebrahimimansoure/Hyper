<template>
    <div>
        <ul class="flex flex-wrap justify-around text-sm md:text-base">
            <!--If active link it has a 2px border bottom -->
            <li :class="{ 'border-b-2 border-cyan-400 cursor-default': isActive('/') }">
                <nuxt-link :class='{"hover:text-cyan-400 animate-item": !isActive("/")}' to="/">Home</nuxt-link>
            </li>
            <li :class="{ 'border-b-2 border-cyan-400 cursor-default': isActive('/lectures') }">
                <nuxt-link :class='{"hover:text-cyan-400 animate-item": !isActive("/lectures")}' to="/lectures">Lectures</nuxt-link>
            </li>
            <li :class="{ 'border-b-2 border-cyan-400 cursor-default': isActive('/speakers') }">
                <nuxt-link :class='{"hover:text-cyan-400 animate-item": !isActive("/speakers")}' to="/speakers">Speakers</nuxt-link>
            </li>
            <li :class="{ 'border-b-2 border-cyan-400 cursor-default': isActive('/social-activities') }">
                <nuxt-link :class='{"hover:text-cyan-400 animate-item": !isActive("/social-activities")}' to="/social-activities">Social activities</nuxt-link>
            </li>
            <li :class="{ 'border-b-2 border-cyan-400 cursor-default': isActive('/about-us') }">
                <nuxt-link :class='{"hover:text-cyan-400 animate-item": !isActive("/about-us")}' to="/about-us">About us</nuxt-link>
            </li>
            <!-- <li :class="{ 'border-b-2 border-cyan-400 cursor-default': isActive('/contact-us') }">
                <nuxt-link :class='{"hover:text-cyan-400 animate-item": !isActive("/contact-us")}' to="/contact-us">Contact us</nuxt-link>
            </li> -->
        </ul>
    </div>
</template>

<script>
// from url find which link is active
export default {
    computed: {
        activeLink() {
            return this.$route.path;
        },
    },
    // nuxt-link to is active if activeLink is eqaul to value of to attribute or it starts with value of to attribute except for the home page
    methods: {
        isActive(to) {
            if (to === "/" && this.activeLink === "/") {
                return true;
            } else if (to !== "/" && this.activeLink.startsWith(to)) {
                return true;
            } else {
                return false;
            }
        },
    },
};
</script>

<style scoped>
.hover-btn:hover {
    @apply text-cyan-400;
}

</style>