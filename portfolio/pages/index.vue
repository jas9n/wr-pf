<template>
  <div id="home">
    <global-navbar />
    <div id="birds" class="fixed inset-0 bg-black h-screen -z-20"></div>
    <div id="overlay" class="fixed inset-0 bg-black opacity-40 h-screen -z-10"></div>
    <home-section id="splash">
      <h2 id="weare" class="text-6xl font-medium overflow-visible">We are WebRising.</h2>
      <p id="built" class="text-xl">Built by high school developers — for you, for free.</p>
    </home-section>
    <home-section>
      <h2 class="text-6xl font-medium overflow-visible">Don't limit your potential.</h2>
      <p class="text-xl">We have the resources and technical expertise to craft streamlined platforms.</p>
    </home-section>
    <home-section>
      <h2 class="text-6xl font-medium overflow-visible">Tailored to your needs.</h2>
      <p class="text-xl">Showcase your products, market your business, or sell your services.</p>
    </home-section>
    <section id="projects" class="h-auto min-h-screen w-full flex justify-center items-center">
      <div id="content" class="w-full max-w-4xl flex flex-col justify-center items-center space-y-8 text-white text-center">
        <h2 class="text-6xl font-medium overflow-visible px-8">Check out our projects.</h2>
        <div id="container" class="w-full flex flex-col justify-center items-center space-y-6">
          <!-- <client/>
        <client/>
        <client/>
        <client/> -->
        </div>
        <nuxt-link to="/projects" class="px-4 py-2 border border-white text-lg text-white rounded ease-in duration-200 hover:bg-white hover:text-black">
          <p>More Work</p>
        </nuxt-link>
      </div>
    </section>
    <home-section>
      <h2 class="text-6xl font-medium overflow-visible">Get started.</h2>
      <!-- <p class="text-xl">Reach out to us to get started.</p> -->
      <p class="text-xl">Let's craft something<span class="text-rose-300"> beautiful</span>.</p>
      <a id="contact" href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=team@webrising.org" target="_blank">
        <button class="px-4 py-2 border border-white text-lg text-white rounded ease-in duration-200 hover:bg-white hover:text-black">
          <p>Contact Us</p>
        </button>
      </a>
    </home-section>
    <global-footer />
  </div>
</template>

<script>
import BIRDS from 'vanta/dist/vanta.birds.min'
import gsap from 'gsap'
import ScrollTrigger from 'gsap/ScrollTrigger'

gsap.registerPlugin(ScrollTrigger)

export default {
  name: 'Home',
  data() {
    return {}
  },
  mounted() {
    gsap
      .timeline({ defaults: { duration: 1 } })
      .from('#splash', { opacity: 0, ease: 'power3.in' }, 0)
      .from('#weare', { y: -30, opacity: 0, ease: 'power2.out' }, 1)
      .from('#built', { y: -20, opacity: 0, ease: 'power2.out' }, 2)

    this.vantaEffect = BIRDS({
      el: '#birds',
      mouseControls: false,
      touchControls: false,
      gyroControls: false,
      maxHeight: 200.0,
      maxWidth: 200.0,
      scale: 1.0,
      scaleMobile: 1.0,
      backgroundColor: 0x000,
      color1: 0xb11e1e,
      color2: 0x217c91,
      birdSize: 1.2,
      wingSpan: 20.0,
      speedLimit: 3.0,
      quantity: 4.0,
    })
  },
}
</script>
