<template>
    <section class="bg-white px-6 pt-20 py-10">
        <div class="container mx-auto max-w-4xl">

        <!-- Header -->
        <h1 class="text-5xl font-bold text-center text-[#333] mb-12 motion-preset-slide-down motion-duration-1500">
            Contact Me
        </h1>

    <!-- Contact Info -->
        <div class="text-center mb-12 motion-preset-expand motion-duration-1500">
            <p class="text-lg text-gray-700 mb-4">
                Feel free to reach out if you’d like to collaborate, have questions, or just want to say hi!
            </p>
            <p class="text-gray-600"><i class="fa-solid fa-envelope"></i> Email: <span class="font-semibold text-blue-600">ralphjosephbatiancila1914@gmail.com</span></p>
            <p class="text-gray-600"><i class="fa-solid fa-location-pin"></i>Location:<span class="text-green-600 font-semibold"> Bukidnon, Philippines</span></p>
            <p class="text-gray-600"><i class="fas fa-phone"></i>Contact:<span class="text-gray-600 font-semibold"> +63 997 795 3461</span></p>
        </div>

        <!-- Contact Form -->
    <form @submit.prevent="sendEmail" class="bg-gray-100 rounded-2xl shadow-lg p-8 space-y-6 motion-preset-blur-right motion-duration-1000">
        <!-- Name -->
        <div>
            <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Name</label>
            <input 
            v-model="form.name" 
            type="text" 
            id="name" 
            placeholder="Your name"
            class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:outline-none">
        </div>

        <!-- Email -->
        <div>
            <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
            <input 
            v-model="form.email"
            type="email" 
            id="email" 
            placeholder="Your email"
            class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:outline-none">
        </div>

        <!-- Message -->
        <div>
            <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
            <textarea 
            v-model="form.message" 
            id="message" 
            rows="4" 
            placeholder="Your message"
            class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:outline-none resize-none"></textarea>
        </div>

        <!-- Submit Button -->
        <button 
        type="submit"
        :disabled="loading" 
            class="w-full bg-blue-700 text-white font-medium py-3 rounded-lg hover:bg-blue-800 transition-colors
                disabled:cursor-not-allowed">
            {{ loading ? "Sending..." : "Send Message" }}
        </button>

        <!-- Validation message -->
        <p v-if="errorMessage" class="text-red-500 text-sm font-medium">
            {{ errorMessage }}
        </p>

        
        <!-- Success Message -->
        <p v-if="successMessage" class="text-green-600 text-sm font-medium">
            {{ successMessage }}
        </p>
    </form>

        </div>
    </section>

    <div class="flex items-center justify-center gap-10 mb-10">
        <!-- Facebook -->
        <a href="https://m.me/ralph.joseph.romano.batiancila" target="_blank" class="group transition-transform duration-700 ease-in-out hover:scale-110">
            <svg xmlns="http://www.w3.org/2000/svg" 
            viewBox="0 0 24 24" width="36" height="36" 
            fill="rgba(24,119,242,1)">
            <path d="M12.001 2C17.6345 2 22.001 6.1265 22.001 11.7C22.001 17.2735 17.6345 21.4 12.001 21.4C11.0233 21.4023 10.0497 21.273 9.10648 21.0155C8.92907 20.9668 8.7403 20.9808 8.57198 21.055L6.58748 21.931C6.34398 22.0386 6.06291 22.018 5.83768 21.8761C5.61244 21.7342 5.47254 21.4896 5.46448 21.2235L5.40998 19.4445C5.40257 19.2257 5.30547 19.0196 5.14148 18.8745C3.19598 17.1345 2.00098 14.6155 2.00098 11.7C2.00098 6.1265 6.36748 2 12.001 2ZM5.99598 14.5365C5.71398 14.984 6.26398 15.488 6.68498 15.1685L9.84048 12.7735C10.0543 12.6122 10.3491 12.6122 10.563 12.7735L12.8995 14.5235C13.2346 14.7749 13.6596 14.8747 14.0716 14.7987C14.4836 14.7227 14.8451 14.4779 15.0685 14.1235L18.006 9.4635C18.288 9.016 17.738 8.512 17.317 8.8315L14.1615 11.2265C13.9476 11.3878 13.6528 11.3878 13.439 11.2265L11.1025 9.4765C10.7673 9.22511 10.3423 9.12532 9.93034 9.2013C9.51834 9.27728 9.15689 9.5221 8.93348 9.8765L5.99598 14.5365Z"></path></svg>
        </a>
        <!-- Whatsapp -->
        <a href="https://wa.me/639977953461" target="_blank" class="group transition-transform duration-700 ease-in-out hover:scale-110">
            <svg xmlns="http://www.w3.org/2000/svg" 
            viewBox="0 0 24 24" width="36" height="36" 
            fill="#25D366"> <!-- WhatsApp green -->
            <path d="M12.001 2C17.5238 2 22.001 6.47715 22.001 12C22.001 17.5228 17.5238 22 12.001 22C10.1671 22 8.44851 21.5064 6.97086 20.6447L2.00516 22L3.35712 17.0315C2.49494 15.5536 2.00098 13.8345 2.00098 12C2.00098 6.47715 6.47813 2 12.001 2ZM8.59339 7.30019L8.39232 7.30833C8.26293 7.31742 8.13607 7.34902 8.02057 7.40811C7.93392 7.45244 7.85348 7.51651 7.72709 7.63586C7.60774 7.74855 7.53857 7.84697 7.46569 7.94186C7.09599 8.4232 6.89729 9.01405 6.90098 9.62098C6.90299 10.1116 7.03043 10.5884 7.23169 11.0336C7.63982 11.9364 8.31288 12.8908 9.20194 13.7759C9.4155 13.9885 9.62473 14.2034 9.85034 14.402C10.9538 15.3736 12.2688 16.0742 13.6907 16.4482C13.6907 16.4482 14.2507 16.5342 14.2589 16.5347C14.4444 16.5447 14.6296 16.5313 14.8153 16.5218C15.1066 16.5068 15.391 16.428 15.6484 16.2909C15.8139 16.2028 15.8922 16.159 16.0311 16.0714C16.0311 16.0714 16.0737 16.0426 16.1559 15.9814C16.2909 15.8808 16.3743 15.81 16.4866 15.6934C16.5694 15.6074 16.6406 15.5058 16.6956 15.3913C16.7738 15.2281 16.8525 14.9166 16.8838 14.6579C16.9077 14.4603 16.9005 14.3523 16.8979 14.2854C16.8936 14.1778 16.8047 14.0671 16.7073 14.0201L16.1258 13.7587C16.1258 13.7587 15.2563 13.3803 14.7245 13.1377C14.6691 13.1124 14.6085 13.1007 14.5476 13.097C14.4142 13.0888 14.2647 13.1236 14.1696 13.2238C14.1646 13.2218 14.0984 13.279 13.3749 14.1555C13.335 14.2032 13.2415 14.3069 13.0798 14.2972C13.0554 14.2955 13.0311 14.292 13.0074 14.2858C12.9419 14.2685 12.8781 14.2457 12.8157 14.2193C12.692 14.1668 12.6486 14.1469 12.5641 14.1105C11.9868 13.8583 11.457 13.5209 10.9887 13.108C10.8631 12.9974 10.7463 12.8783 10.6259 12.7616C10.2057 12.3543 9.86169 11.9211 9.60577 11.4938C9.5918 11.4705 9.57027 11.4368 9.54708 11.3991C9.50521 11.331 9.45903 11.25 9.44455 11.1944C9.40738 11.0473 9.50599 10.9291 9.50599 10.9291C9.50599 10.9291 9.74939 10.663 9.86248 10.5183C9.97128 10.379 10.0652 10.2428 10.125 10.1457C10.2428 9.95633 10.2801 9.76062 10.2182 9.60963C9.93764 8.92565 9.64818 8.24536 9.34986 7.56894C9.29098 7.43545 9.11585 7.33846 8.95659 7.32007C8.90265 7.31384 8.84875 7.30758 8.79459 7.30402C8.66053 7.29748 8.5262 7.29892 8.39232 7.30833L8.59339 7.30019Z"></path>
            </svg>
        </a>
        <!-- instagram -->
        <a href="https://www.instagram.com/ralphnotfound_/" target="_blank" class="group transition-transform duration-700 ease-in-out hover:scale-110">
            <svg xmlns="http://www.w3.org/2000/svg" 
            viewBox="0 0 24 24" width="36" height="36">
                <defs>
                    <linearGradient id="instaGradient" x1="0%" y1="0%" x2="100%" y2="100%">
                        <stop offset="0%" stop-color="rgb(131,58,180)" />   <!-- Purple -->
                        <stop offset="50%" stop-color="rgb(193,53,132)" />  <!-- Pink -->
                        <stop offset="75%" stop-color="rgb(253,29,29)" />   <!-- Red -->
                        <stop offset="100%" stop-color="rgb(252,176,69)" /> <!-- Orange/Yellow -->
                    </linearGradient>
                </defs>
                <path fill="url(#instaGradient)" d="M13.0281 2.00073C14.1535 2.00259 14.7238 2.00855 15.2166 2.02322L15.4107 2.02956C15.6349 2.03753 15.8561 2.04753 16.1228 2.06003C17.1869 2.1092 17.9128 2.27753 18.5503 2.52503C19.2094 2.7792 19.7661 3.12253 20.3219 3.67837C20.8769 4.2342 21.2203 4.79253 21.4753 5.45003C21.7219 6.0867 21.8903 6.81337 21.9403 7.87753C21.9522 8.1442 21.9618 8.3654 21.9697 8.58964L21.976 8.78373C21.9906 9.27647 21.9973 9.84686 21.9994 10.9723L22.0002 11.7179C22.0003 11.809 22.0003 11.903 22.0003 12L22.0002 12.2821L21.9996 13.0278C21.9977 14.1532 21.9918 14.7236 21.9771 15.2163L21.9707 15.4104C21.9628 15.6347 21.9528 15.8559 21.9403 16.1225C21.8911 17.1867 21.7219 17.9125 21.4753 18.55C21.2211 19.2092 20.8769 19.7659 20.3219 20.3217C19.7661 20.8767 19.2069 21.22 18.5503 21.475C17.9128 21.7217 17.1869 21.89 16.1228 21.94C15.8561 21.9519 15.6349 21.9616 15.4107 21.9694L15.2166 21.9757C14.7238 21.9904 14.1535 21.997 13.0281 21.9992L12.2824 22C12.1913 22 12.0973 22 12.0003 22L11.7182 22L10.9725 21.9993C9.8471 21.9975 9.27672 21.9915 8.78397 21.9768L8.58989 21.9705C8.36564 21.9625 8.14444 21.9525 7.87778 21.94C6.81361 21.8909 6.08861 21.7217 5.45028 21.475C4.79194 21.2209 4.23444 20.8767 3.67861 20.3217C3.12278 19.7659 2.78028 19.2067 2.52528 18.55C2.27778 17.9125 2.11028 17.1867 2.06028 16.1225C2.0484 15.8559 2.03871 15.6347 2.03086 15.4104L2.02457 15.2163C2.00994 14.7236 2.00327 14.1532 2.00111 13.0278L2.00098 10.9723C2.00284 9.84686 2.00879 9.27647 2.02346 8.78373L2.02981 8.58964C2.03778 8.3654 2.04778 8.1442 2.06028 7.87753C2.10944 6.81253 2.27778 6.08753 2.52528 5.45003C2.77944 4.7917 3.12278 4.2342 3.67861 3.67837C4.23444 3.12253 4.79278 2.78003 5.45028 2.52503C6.08778 2.27753 6.81278 2.11003 7.87778 2.06003C8.14444 2.04816 8.36564 2.03847 8.58989 2.03062L8.78397 2.02433C9.27672 2.00969 9.8471 2.00302 10.9725 2.00086L13.0281 2.00073ZM12.0003 7.00003C9.23738 7.00003 7.00028 9.23956 7.00028 12C7.00028 14.7629 9.23981 17 12.0003 17C14.7632 17 17.0003 14.7605 17.0003 12C17.0003 9.23713 14.7607 7.00003 12.0003 7.00003ZM12.0003 9.00003C13.6572 9.00003 15.0003 10.3427 15.0003 12C15.0003 13.6569 13.6576 15 12.0003 15C10.3434 15 9.00028 13.6574 9.00028 12C9.00028 10.3431 10.3429 9.00003 12.0003 9.00003ZM17.2503 5.50003C16.561 5.50003 16.0003 6.05994 16.0003 6.74918C16.0003 7.43843 16.5602 7.9992 17.2503 7.9992C17.9395 7.9992 18.5003 7.4393 18.5003 6.74918C18.5003 6.05994 17.9386 5.49917 17.2503 5.50003Z"></path>
            </svg>
        </a>
    </div>



</template>

<script>
import emailjs from "emailjs-com"

export default {
    data() {
        return {
            form: {
            name: "",
            email: "",
            message: "",
        },
            loading: false,
            errorMessage: "",
            successMessage: "",
        };
    },
    methods: {
        async sendEmail() {
            try {

                this.errorMessage = "";
                this.successMessage = "";

                if (!this.form.name || !this.form.email || !this.form.message) {
                    this.showTemporaryMessage('errorMessage', "Please fill in all the fields before sending.")
                    return
                }
                this.loading = true

                const templateParams = {
                    name: this.form.name,
                    email: this.form.email,
                    message: this.form.message,
                    time: new Date().toLocaleString(), // auto-adds the time
                };

                await emailjs.send(
                import.meta.env.VITE_EMAILJS_SERVICE_ID,   // replace with your EmailJS service ID
                import.meta.env.VITE_EMAILJS_TEMPLATE_ID,  // replace with your EmailJS template ID
                templateParams,
                import.meta.env.VITE_EMAILJS_PUBLIC_KEY    // replace with your EmailJS public key
                );

                this.showTemporaryMessage('successMessage' , "✅ Message sent successfully!");
                this.form = { name: "", email: "", message: "" }; // reset form
            } catch (error) {
                console.error("EmailJS Error:", error);
            this.status = "❌ Failed to send message. Try again.";
            } finally {
                this.loading = false
            }
        },

        showTemporaryMessage(type, text) {
            this[type] = text
            setTimeout(() => {
                this[type] = ''
            },3000)
        }
    },
};
</script>
