<template>
    <div class="bg-gray-900 text-white min-h-screen">
        <!-- Header Section -->
        <header class="w-full h-[80px] bg-gray-800 flex items-center justify-between px-22 shadow-lg  fixed">
            <h1 class="text-2xl font-bold">
                <a href="#">
                    Ramones, Eric, Jr. M.
                </a>
            </h1>
            <nav>
                <ul class="flex space-x-10 text-lg">
                    <li class="hover:text-orange-400 cursor-pointer"><a href="#about">About</a></li>
                    <li class="hover:text-orange-400 cursor-pointer"><a href="#projects">Projects</a></li>
                    <li class="hover:text-orange-400 cursor-pointer"><a href="#contacts">Contacts</a></li>
                </ul>
            </nav>
        </header>

        <!-- Hero Section -->
        <section id="about" class="flex flex-col md:flex-row items-center justify-between px-22 py-25">
            <div class="text-left">
                <h2 class="text-5xl font-semibold">Hello.</h2>
                <h3 class="text-4xl mt-4">I'm Eric, Jr.</h3>
                <h1 class="text-6xl font-bold mt-4">
                    a <span class="text-orange-400">
                        <!-- Apply transition class here -->
                        <transition name="fade" mode="out-in">
                            <span :key="rotatingText">{{ rotatingText }}</span>
                        </transition>
                    </span>
                </h1>
                
                <div class="mt-6 space-x-4">
                    <button class="px-6 py-3 border-2 border-white text-white font-semibold rounded-lg hover:bg-white hover:text-gray-900">
                        Download Resume
                    </button>
                </div>
            </div>
            <div class="mt-10 md:mt-0">
                <img src="../img/ericjr..png" alt="Profile" class="w-auto h-auto">
            </div>
        </section>

        <!-- Skills Section -->
        <section class="bg-gray-800 py-8 ">
            <div class="flex justify-center space-x-10 text-gray-400 text-lg">
                <span class="hover:text-orange-400 cursor-pointer">HTML5</span>
                <span class="hover:text-orange-400 cursor-pointer">CSS</span>
                <span class="hover:text-orange-400 cursor-pointer">JavaScript</span>
                <span class="hover:text-orange-400 cursor-pointer">Laravel</span>
                <span class="hover:text-orange-400 cursor-pointer">PHP</span>
                <span class="hover:text-orange-400 cursor-pointer">MYSQL</span>
            </div>
        </section>

        <section class="bg-gray-900 text-white py-16 px-6">
            <div class="max-w-6xl mx-auto">
                <h2 class="text-4xl font-bold ">Skill-Set</h2>
                <div class="w-20 h-1 bg-white mt-2"></div>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 mt-10">
                    

                    <div class="bg-gray-800 p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold mt-4">Figma Design</h3>
                        <p class="text-gray-400 mt-2">Having average knowledge in using Figma. Knowing its basic tools and its uses</p>
                    </div>

                    <div class="bg-gray-800 p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold mt-4">Back-end Development</h3>
                        <p class="text-gray-400 mt-2">Always assigned in back-end in every school project. Have average knowledge about Laravel PHP and some familiarization in SQL databases.</p>
                    </div>

                    <div class="bg-gray-800 p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold mt-4">Web Development</h3>
                        <p class="text-gray-400 mt-2">Have Average knowledge in web development knowing Vue JS and Tailwind. Also willing to learn and adapt new technologies such as React.</p>
                    </div>

                </div>
            </div>
            
        </section>


        <!-- Projects Section -->
        <section id="projects" class="py-20 text-center bg-gray-800">
            <h2 class="text-4xl font-semibold mb-4 transition duration-300 hover:text-blue-400">Projects</h2>
            <div class="w-24 h-1 bg-white mx-auto mb-8 transition duration-300 hover:bg-blue-400 "></div>

            <div class="flex flex-col items-center space-y-10">

                <!-- Project 1: Lendcash Microfinance System -->
                <div class="flex flex-row items-center max-w-4xl text-left space-x-6">
                    <img src="../img/lendcash.png" alt="Lendcash Microfinance System" class="rounded-lg shadow-lg w-1/2">
                    <div class="w-1/2">
                        <h3 class="text-lg font-semibold text-blue-400">Lendcash Microfinance System</h3>
                        <p class="text-gray-400 mt-2">
                            An Online Microfinance Lending System designed to empower individuals and small businesses by 
                            providing quick and easy access to financial services, made with Vue JS and PHP Laravel with MYSQL Database.
                        </p>
                        <a href="https://lendcash.netlify.app/" class="inline-block mt-4 px-4 py-2 border border-blue-400 text-blue-400 rounded-lg hover:bg-blue-400 hover:text-white">
                            Learn More
                        </a>
                    </div>
                </div>

                <hr class="w-3/4 border-t border-gray-600 my-10">

                <!-- Project 2: Point of Sales System -->
                <div class="flex flex-row items-center max-w-4xl text-left space-x-6">
                    <div class="w-1/2">
                        <h3 class="text-lg font-semibold text-blue-400">Point of Sales System</h3>
                        <p class="text-gray-400 mt-2">
                            An <span class="text-red-500">unfinished</span>
                            POS system that is designed to manage inventory, 
                            and generate insightful sales reports efficiently made with C# and SQL.
                        </p>
                    </div>
                    <img src="../img/pos.png" alt="Point of Sales System" class="rounded-lg shadow-lg w-1/2">
                </div>

                <hr class="w-3/4 border-t border-gray-600 my-10">

                <!-- Project 3: E-commerce Design in Figma -->
                <div class="flex flex-row items-center max-w-4xl text-left space-x-6">
                    <img src="../img/figmaproj.png" alt="E-commerce Design in Figma" class="rounded-lg shadow-lg w-1/2">
                    <div class="w-1/2">
                        <h3 class="text-lg font-semibold text-blue-400">E-commerce Design in Figma</h3>
                        <p class="text-gray-400 mt-2">
                            A school project E-commerce design created in Figma, 
                            focusing on UI/UX optimization for better user engagement.
                        </p>
                        <a href="https://www.figma.com/proto/kgktoy6TuZxGDYpOQ3ARL4/gunshop?node-id=31-75&p=f&t=zTpXGcAvr9H24vEE-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=31%3A75&show-proto-sidebar=1" 
                            class="inline-block mt-4 px-4 py-2 border border-blue-400 text-blue-400 rounded-lg hover:bg-blue-400 hover:text-white">
                            Learn More
                        </a>
                    </div>
                </div>

            </div>
        </section>

        <section id="projects" class="py-20 text-center bg-gray-800">
            <h2 class="text-4xl font-semibold mb-4 transition duration-300 hover:text-blue-400">Projects</h2>
            <div class="w-24 h-1 bg-white mx-auto mb-8 transition duration-300 hover:bg-blue-400 "></div>

            <div class="flex flex-col items-center space-y-10">

                <!-- Project 1: Lendcash Microfinance System -->
                <div class="flex flex-row items-center max-w-4xl text-left space-x-6">
                    <img src="../img/lendcash.png" alt="Lendcash Microfinance System" class="rounded-lg shadow-lg w-1/2">
                    <div class="w-1/2">
                        <h3 class="text-lg font-semibold text-blue-400">Lendcash Microfinance System</h3>
                        <p class="text-gray-400 mt-2">
                            An Online Microfinance Lending System designed to empower individuals and small businesses by 
                            providing quick and easy access to financial services, made with Vue JS and PHP Laravel with MYSQL Database.
                        </p>
                        <a href="https://lendcash.netlify.app/" class="inline-block mt-4 px-4 py-2 border border-blue-400 text-blue-400 rounded-lg hover:bg-blue-400 hover:text-white">
                            Learn More
                        </a>
                    </div>
                </div>

                <hr class="w-3/4 border-t border-gray-600 my-10">

            </div>
        </section>

        <section id="contacts" class="py-20 text-center bg-gray-900 text-white">
            <h2 class="text-4xl font-semibold mb-4 transition duration-300 hover:text-blue-400">Contact Me</h2>
            <div class="w-24 h-1 bg-white mx-auto mb-8 transition duration-300 hover:bg-blue-400"></div>

            <div class="flex flex-col items-center space-y-10">
                <div class="flex flex-row items-center max-w-4xl text-left space-x-6">
                    <div class="w-1/2 space-y-6">
                        <div class="space-y-4">
                            <div class="flex items-center space-x-4">
                                <span class="text-lg text-gray-300">📧 ericramones1253@gmail.com</span>
                            </div>
                            <div class="flex items-center space-x-4">
                                <span class="text-lg text-gray-300">📍 Talomo Proper School Site, Davao City</span>
                            </div>
                            <div class="flex items-center space-x-4">
                                <span class="text-lg text-gray-300">📞 +63 9087373926</span>
                            </div>
                        </div>
                    </div>

                    <!-- Contact Form -->
                    <div class="w-1/2">
                        <form action="https://formsubmit.co/c7e8a2d12c5637a4c1574d9f0549d8c2" method="POST" class="space-y-5 bg-gray-800 p-6 rounded-lg shadow-lg">
                            <input type="email" name="email" required placeholder="📧 Your Email" class="w-full p-3 bg-gray-700 text-white border border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500">
                            <textarea name="message" rows="4" required placeholder="💬 Your Message" class="w-full p-3 bg-gray-700 text-white border border-gray-600 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500"></textarea>
                            <button type="submit" class="w-full bg-blue-500 text-white py-3 rounded-md hover:bg-blue-600 transition">
                                🚀 Send Message
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </section>

    </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

// Rotating words logic
const words = ["Web Developer.", "Programmer.", "Designer.", "Kupal."];
const rotatingText = ref(words[0]);
let index = 0;

onMounted(() => {
    setInterval(() => {
        index = (index + 1) % words.length;
        rotatingText.value = words[index];
    }, 2000);
});
</script>


<style scoped>
/* Add a simple fade transition */
.fade-enter-active, .fade-leave-active {
    transition: opacity 1s ease-in-out;
}
.fade-enter, .fade-leave-to  {
    opacity: 0;
}

</style>
