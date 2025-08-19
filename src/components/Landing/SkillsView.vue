<template>
    <section class="bg-white px-6 py-20">
        <div class="container mx-auto max-w-6xl">

            <!-- Header -->
            <h1 class="text-5xl font-bold text-center text-[#333] mb-12 motion-preset-slide-down motion-duration-1500">
                My Projects
            </h1>


        <!-- Projects Grid -->
            <div class="grid grid-cols-2 md:grid-cols-2 lg:grid-cols-2 gap-10 motion-preset-slide-up motion-duration-2000">
        
            <!-- Project Card -->
                <div v-for="(project, index) in projects" :key="index" class="bg-gray-100 rounded-2xl overflow-hidden shadow-lg transition-transform duration-500 hover:scale-105">
                    <img :src="project.image" :alt="project.title" class="w-full h-48 object-cover"/>
                    <div class="p-6">
                        <h2 class="text-2xl font-semibold text-gray-800 mb-2">{{ project.title }}</h2>
                        <p class="text-gray-600 mb-4">{{ project.description }}</p>
                        <a :href="project.link" target="_blank" class="inline-block text-white bg-blue-700 px-4 py-2 rounded-full hover:bg-blue-800 transition-colors">View Project</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import capstoneImg from '@/assets/img/Capstone.png'
import portfolioImg from '@/assets/img/Portfolio.png'

export default {
    data() {
        return {
            projects: [
            {
                title: "Capstone School Website",
                description: "A dynamic school website built with Vue.js and Django backend.",
                image: capstoneImg,
                link: "https://github.com/Ralphwasnotfound/Capstone"
            },
            {
            title: "Portfolio Site",
            description: "My personal portfolio to showcase my projects and skills.",
            image: portfolioImg,
            link: "https://github.com/Ralphwasnotfound/Portfolio"
            },
        // Add more projects here
            ]
        }
    }
}
</script>

<style>
    /* Optional */
</style>