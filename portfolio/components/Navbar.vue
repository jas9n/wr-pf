<template>
    <div>
        <div id="nav" class="absolute inset-0 w-full h-20 text-white flex justify-center items-center z-40 bg-black">
            <div id="content" class="w-full h-full flex justify-between items-center px-8">
                <div id="title" class="h-10">
                    <nuxt-link to="/">
                        <h1 class="text-3xl  font-semibold mx-1 text-white overflow-visible">WebRising</h1>
                    </nuxt-link>
                </div>
                <ul id="links" class="hidden justify-center items-center space-x-10 text-lg  text-white md:flex">
                    <li>About Us</li>
                    <li>Our Work</li>
                    <li>Our Services</li>
                </ul>
                <a id="contact" class="hidden md:block" href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=team@webrising.org" target="_blank">
                    <button class="px-4 py-2 border border-white text-base text-white rounded-full transition duration-200 hover:bg-white hover:text-black">
                        <p>Contact Us</p>
                    </button>
                </a>
                <div id="toggle" class="flex justify-center items-center space-x-2 z-40 md:hidden">
                    <div id="menu-icon" class="cursor-pointer" @click="toggleMenu" v-if="!menu">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8  text-white" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd" />
                        </svg>
                    </div>
                    <div id="close" class="cursor-pointer" @click="toggleMenu" v-else>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-white" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd" />
                        </svg>
                    </div>  
                </div>
            </div>
        </div>
        <div id="menu" v-if="menu" class="absolute right-0 h-screen w-full text-white text-xl z-30 pl-16 bg-black md:hidden">
            <ul id="links" class="h-full flex flex-col justify-center items-start space-y-10 text-lg text-white">
                <li>About Us</li>
                <li>Our Work</li>
                <li>Our Services</li>
                <a id="contact" href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=team@webrising.org" target="_blank">
                    <li>Contact Us</li>
                </a>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: "Navbar",
    data() {
        return {
            menu: false
        }
    },
    methods: {
        toggleMenu() {
            if (!this.menu) {
                this.menu = true
            } else {
                this.menu = false
            }
        }
    }

}
</script>