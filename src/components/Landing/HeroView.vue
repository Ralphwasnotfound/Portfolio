<template>
    <section class="bg-white px-6 py-16">
        <div class="container mx-auto flex flex-col md:flex-row items-center justify-between px-20">
        
            <!-- Left: Text -->
        <div class="text-center md:text-left max-w-lg">
            <h1 class="text-5xl text-[#333]  font-bold mb-4 motion-preset-slide-right motion-duration-1000">
                Hi, <br />
                I’m <span class="text-blue-700 font-bold motion-preset-focus motion-duration-2000">Ralph Joseph Batiancila
                </span>
            </h1>
            <p class="text-4xl text-[#333] mb-6 motion-preset-focus motion-preset-slide-right motion-duration-1500">
                Web Developer/Programmer
            </p>

            <!-- Button -->
                <router-link to="/contact" class="inline-block text-white bg-blue-700 hover:bg-blue-800 font-medium rounded-full text-sm px-5 py-2.5 text-center transition-transform duration-700 ease-in-out hover:scale-110 motion-preset-slide-right motion-duration-2000">
                    Contact Me
                </router-link>
            </div>

            <!-- Right: Image with Blob Background -->
            <div   div class="relative w-[300px] h-[300px] flex-shrink-0 group overflow-hidden motion-preset-expand motion-duration-2000 drop-shadow-lg ">
            <!-- Blob Shape Background -->
            <div class="absolute inset-0 bg-gradient-to-b from-blue-600 to-blue-400 rounded-[50%_10%_70%_70%/50%_50%_80%_80%] transition-transform duration-700 ease-in-out group-hover:scale-90" ></div>

            <!-- Profile Image inside same blob -->
                <img 
                src="@/assets/img/Parsh.png" 
                alt="Profile" 
                class="relative w-full h-full object-cover rounded-[30%_30%_70%_70%/40%_40%_80%_80%] transition-transform duration-700 ease-in-out group-hover:scale-90"/>
            </div>
            
        </div>
    </section>

    <div class="flex justify-start items-center gap-10 px-28">
        <a href="https://www.linkedin.com/in/ralph-joseph-batiancila-980451322/" target="_blank" class="motion-preset-shrink motion-duration-1000">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="35" height="35" fill="rgb(10,102,194)"><path d="M6.94048 4.99993C6.94011 5.81424 6.44608 6.54702 5.69134 6.85273C4.9366 7.15845 4.07187 6.97605 3.5049 6.39155C2.93793 5.80704 2.78195 4.93715 3.1105 4.19207C3.43906 3.44699 4.18654 2.9755 5.00048 2.99993C6.08155 3.03238 6.94097 3.91837 6.94048 4.99993ZM7.00048 8.47993H3.00048V20.9999H7.00048V8.47993ZM13.3205 8.47993H9.34048V20.9999H13.2805V14.4299C13.2805 10.7699 18.0505 10.4299 18.0505 14.4299V20.9999H22.0005V13.0699C22.0005 6.89993 14.9405 7.12993 13.2805 10.1599L13.3205 8.47993Z"></path></svg>
        </a>

        <a href="https://www.facebook.com/ralph.joseph.romano.batiancila/" class="motion-preset-shrink motion-duration-1000" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" 
            viewBox="0 0 24 24" width="36" height="36" 
            fill="rgba(24,119,242,1)">
            <path d="M12.001 2C6.47813 2 2.00098 6.47715 2.00098 12C2.00098 16.9913 5.65783 21.1283 10.4385 21.8785V14.8906H7.89941V12H10.4385V9.79688C10.4385 7.29063 11.9314 5.90625 14.2156 5.90625C15.3097 5.90625 16.4541 6.10156 16.4541 6.10156V8.5625H15.1931C13.9509 8.5625 13.5635 9.33334 13.5635 10.1242V12H16.3369L15.8936 14.8906H13.5635V21.8785C18.3441 21.1283 22.001 16.9913 22.001 12C22.001 6.47715 17.5238 2 12.001 2Z"></path>
            </svg>
        </a>

        <a href="https://gitlab.com/ralphnotfound-group/Ralphnotfound-project" class="motion-preset-shrink motion-duration-1000" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="35" height="35" fill="rgb(252,109,38)"><path d="M21.6634 9.98681L21.6354 9.91518L18.9164 2.8208C18.8612 2.68166 18.7634 2.56353 18.6371 2.48326C18.5098 2.40292 18.3607 2.36406 18.2104 2.37206C18.0601 2.38006 17.9159 2.43452 17.7979 2.52792C17.6809 2.62169 17.5966 2.75 17.5569 2.89453L15.7187 8.52037H8.28157L6.44336 2.89453C6.40366 2.75 6.31934 2.62169 6.20241 2.52792C6.08487 2.43389 5.94083 2.37903 5.79052 2.37102C5.64021 2.36301 5.49116 2.40226 5.36429 2.48326C5.2374 2.5632 5.13921 2.6814 5.08388 2.8208L2.36183 9.9245L2.33379 9.99512C1.94304 11.0182 1.895 12.1406 2.19691 13.1933C2.49882 14.2461 3.13436 15.1724 4.00794 15.8329L4.01832 15.8401L4.04221 15.8588L8.18917 18.9631L10.2393 20.5157L11.4856 21.4597C11.6319 21.5704 11.8104 21.6302 11.9939 21.6302C12.1774 21.6302 12.3559 21.5704 12.5023 21.4597L13.7486 20.5157L15.7997 18.9631L19.9706 15.8401L19.9819 15.8318C20.8585 15.1719 21.4966 14.2449 21.7999 13.1904C22.1033 12.1361 22.0553 11.0116 21.6634 9.98681Z"></path></svg>
        </a>

        <a href="https://github.com/Ralphwasnotfound" target="_blank" class="motion-preset-shrink motion-duration-1000">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="36" height="36" fill="rgba(0,0,0,1)"><path d="M12.001 2C6.47598 2 2.00098 6.475 2.00098 12C2.00098 16.425 4.86348 20.1625 8.83848 21.4875C9.33848 21.575 9.52598 21.275 9.52598 21.0125C9.52598 20.775 9.51348 19.9875 9.51348 19.15C7.00098 19.6125 6.35098 18.5375 6.15098 17.975C6.03848 17.6875 5.55098 16.8 5.12598 16.5625C4.77598 16.375 4.27598 15.9125 5.11348 15.9C5.90098 15.8875 6.46348 16.625 6.65098 16.925C7.55098 18.4375 8.98848 18.0125 9.56348 17.75C9.65098 17.1 9.91348 16.6625 10.201 16.4125C7.97598 16.1625 5.65098 15.3 5.65098 11.475C5.65098 10.3875 6.03848 9.4875 6.67598 8.7875C6.57598 8.5375 6.22598 7.5125 6.77598 6.1375C6.77598 6.1375 7.61348 5.875 9.52598 7.1625C10.326 6.9375 11.176 6.825 12.026 6.825C12.876 6.825 13.726 6.9375 14.526 7.1625C16.4385 5.8625 17.276 6.1375 17.276 6.1375C17.826 7.5125 17.476 8.5375 17.376 8.7875C18.0135 9.4875 18.401 10.375 18.401 11.475C18.401 15.3125 16.0635 16.1625 13.8385 16.4125C14.201 16.725 14.5135 17.325 14.5135 18.2625C14.5135 19.6 14.501 20.675 14.501 21.0125C14.501 21.275 14.6885 21.5875 15.1885 21.4875C19.259 20.1133 21.9999 16.2963 22.001 12C22.001 6.475 17.526 2 12.001 2Z"></path></svg>
        </a>
    </div>
</template>

<script>
export default {}
</script>
