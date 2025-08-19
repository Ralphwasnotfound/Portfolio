<template>
<section class="bg-white px-6 py-20">
    <div class="container mx-auto max-w-5xl">

    <!-- Header -->
        <h1 class="text-5xl font-bold text-[#333] mb-8 text-center motion-preset-slide-down motion-duration-1500">
            About Me
        </h1>

    <!-- About Me Text -->
        <div class="mb-12 text-center md:text-left">
            <p class="text-xl text-center text-gray-700 mb-4 motion-scale-in-[0.5] motion-duration-1000">
                Hi, I'm <span class="font-bold text-blue-700">Ralph Joseph Batiancila</span>, a passionate Web Developer/Programmer.  
                I love creating interactive web applications and learning new technologies to improve my skills.
            </p>
            <p class="text-gray-600 motion-scale-in-[0.5] motion-delay-[0.25s] text-center">
                I enjoy solving problems, building clean and efficient code, and continuously challenging myself to grow as a developer.
            </p>
        </div>

    <!-- Skills Section -->
        <div class="mb-12 pt-24">
            <h2 class="text-3xl font-semibold text-center mb-8 motion-preset-slide-down motion-duration-1500">My Skills</h2>

            <div class="grid grid-cols-2 md:grid-cols-4 gap-10 justify-items-center">

            <!-- HTML -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-right motion-duration-1500">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="rgb(227,79,38)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="25.12"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">90%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">HTML</span>
                </div>

            <!-- CSS -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-right motion-duration-1500">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="rgb(38, 77, 228)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="37.68"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">85%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">CSS</span>
                </div>

            <!-- JavaScript -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-left motion-duration-1500">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="rgb(247, 223, 30)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="50.24"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">80%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">JavaScript</span>
                </div>

            <!-- Vue.js -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-left motion-duration-2000">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="rgb(65, 184, 131)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="62.8"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">75%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">Vue.js</span>
                </div>

            <!-- Node.js -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-right motion-duration-2000">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="rgb(83, 165, 83)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="75.36"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">70%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">Node.js</span>
                </div>

            <!-- PYTHON -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-right motion-duration-2000">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                        <defs>
                            <linearGradient id="htmlGradient" x1="0%" y1="0%" x2="100%" y2="0%">
                                <stop offset="0%" stop-color="#ffd946"/>
                                <stop offset="100%" stop-color="#3472a3"/>
                            </linearGradient>
                        </defs>

                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="url(#htmlGradient)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="87.92"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">65%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">Python</span>
                </div>

            <!-- DJANGO -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-left motion-duration-1500">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="rgb(83, 165, 83)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="125.6"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">50%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">Django</span>
                </div>

            <!-- MySQL -->
                <div class="cursor-pointer group flex flex-col items-center relative transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-left motion-duration-2000">
                    <svg viewBox="0 0 100 100" class="w-24 h-24">
                    <!-- Background circle -->
                    <circle cx="50" cy="50" r="40" stroke="#e5e7eb" stroke-width="8" fill="none"/>
                    <!-- Progress circle -->
                    <circle cx="50" cy="50" r="40" stroke="rgb(68, 121, 161)" stroke-width="8" fill="none"
                    stroke-dasharray="251.2" stroke-dashoffset="75.36"
                    stroke-linecap="round" transform="rotate(-90 50 50)"/>
                    <!-- Percentage Text -->
                    <text x="50" y="50" text-anchor="middle" dominant-baseline="middle"
                    class="text-xl font-bold fill-gray-700">70%</text>
                    </svg>
                    <span class="mt-2 font-medium text-gray-700">MySql</span>
                </div>

        </div>
    </div>

    <!-- Personal Statement -->
        <div class="text-center md:text-left motion-preset-slide-up motion-duration-1500 pt-24">
            <h2 class="text-3xl font-semibold text-[#333] mb-4">A Little More About Me</h2>
                <p class="text-gray-700 mb-2">
                    I enjoy building web applications that solve real problems. I’m a fast learner, highly motivated, and always seeking opportunities to grow.
                </p>
                <p class="text-gray-700">
                    When I’m not coding, I enjoy running, gaming, and exploring new technologies to keep myself updated in the fast-changing world of development.
                </p>
            </div>
        </div>
    </section>
</template>

<script>
export default {}
</script>
