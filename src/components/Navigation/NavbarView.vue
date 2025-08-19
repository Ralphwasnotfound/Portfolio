<template>
    <nav class="bg-white flex justify-between items-center px-8 py-4 drop-shadow-lg">
    <!-- Logo -->
            <div class="flex items-center gap-3">
                <span class="cursor-pointer relative text-[#333] hover:text-[#2563EB] font-bold text-lg after:content-[''] after:absolute after:left-0 after:-bottom-1 after:w-0 after:h-[2px] after:bg-[#2563EB] after:transition-all after:duration-300 hover:after:w-full">
                    Ralph Joseph
                </span>
            </div>

    <!-- Links -->
    <div class="flex items-center gap-8 text-[#333] font-medium">
            <router-link to="/" class="relative text-[#333] hover:text-[#2563EB] font-bold text-lg after:content-[''] after:absolute after:left-0 after:-bottom-1 after:w-0 after:h-[2px] after:bg-[#2563EB] after:transition-all after:duration-300 hover:after:w-full">Home</router-link>
            <router-link to="/about" class="relative text-[#333] hover:text-[#2563EB] font-bold text-lg after:content-[''] after:absolute after:left-0 after:-bottom-1 after:w-0 after:h-[2px] after:bg-[#2563EB] after:transition-all after:duration-300 hover:after:w-full">About</router-link>
            <router-link to="/projects" class="relative text-[#333] hover:text-[#2563EB] font-bold text-lg after:content-[''] after:absolute after:left-0 after:-bottom-1 after:w-0 after:h-[2px] after:bg-[#2563EB] after:transition-all after:duration-300 hover:after:w-full">Projects</router-link>
            <router-link to="/contact" class="relative text-[#333] hover:text-[#2563EB] font-bold text-lg after:content-[''] after:absolute after:left-0 after:-bottom-1 after:w-0 after:h-[2px] after:bg-[#2563EB] after:transition-all after:duration-300 hover:after:w-full">Contact</router-link>
        </div>
    </nav>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
/* Optional: highlight active route */
.router-link-exact-active {
    color: #2563EB; /* yellow-400 */
    font-weight: 600;
    position: relative;
}

.router-link-exact-active::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: -4px; /* adjust to match your hover underline */
    width: 100%;
    height: 2px;
    background: #2563EB;
    transition: width 0.3s;
}

</style>
