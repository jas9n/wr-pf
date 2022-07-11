<template>
    <div id="footer">
        <div id="container" class="w-full h-64 flex flex-col justify-between items-start p-12 overflow-hidden md:flex-row sm:h-56 md:h-44 md:px-16 lg:px-20">
            <div id="links" class="overflow-visible">
                <a id="contact" href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=team@webrising.org" target="_blank">
                    <h5 class="text-white text-xl font-medium">team@webrising.org</h5>
                </a>
                <a id="gitlogo" href="https://github.com/web-rising" target="_blank">
                    <img src="@/assets/icons/github.svg" alt="" class="h-16 w-auto"/>
                </a>
            </div>
            <ul id="nav-list" class="grid grid-cols-2 grid-flow-row gap-x-20 gap-y-4 justify-center items-center text-lg overflow-visible text-white sm:flex sm:space-x-12 sm:gap-x-0 sm:gap-y-0">
                <li class="relative table-cell"><nuxt-link to="/about" id="underline" class="relative inline-block pb-1">About Us</nuxt-link></li>
                <li class="relative table-cell"><nuxt-link to="/projects" id="underline" class="relative inline-block pb-1">Our Work</nuxt-link></li>
                <li class="relative table-cell"><nuxt-link to="/services" id="underline" class="relative inline-block pb-1">Our Services</nuxt-link></li>
                <li class="relative table-cell"><a id="underline" href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=team@webrising.org" target="_blank" class="relative inline-block pb-1">Contact Us</a></li>
            </ul>
        </div>
        <h6 id="copyright" class="text-zinc-500 text-sm font-semibold mx-12 mb-8 lg:mx-20">Copyright 2022 WebRising All Rights Reserved</h6>
    </div>
</template>

<script>
export default {
    name:"Footer"
}
</script>

<style scoped>
#underline:after {    
  background: none repeat scroll 0 0 transparent;
  bottom: 0;
  content: "";
  display: block;
  height: 1.5px;
  border-radius: 0.6px;
  left: 50%;
  position: absolute;
  background: rgb(253 164 175);
  transition: width 0.4s ease 0s, left 0.4s ease 0s;
  width: 0;
}
#underline:hover:after { 
  width: 100%; 
  left: 0; 
}
</style>