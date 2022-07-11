<template>
  <div id="home">
    <global-navbar />
    <div id="birds" class="fixed inset-0 bg-black h-screen -z-20"></div>
    <!-- <div id="overlay" class="fixed inset-0 bg-black opacity-60 h-screen -z-10"></div> -->
    <home-section>
      <h2 class="text-6xl font-medium overflow-visible">We are WebRising.</h2>
      <p class="text-xl ml-1">Built by high school developers — for you, for free.</p>
    </home-section>
    <home-section>
      <h2 class="text-6xl font-medium overflow-visible">Don't limit your potential.</h2>
      <p class="text-xl ml-1">We have the resources and technical expertise to craft your streamlined platform.</p>
    </home-section>
    <home-section>
      <h2 class="text-6xl font-medium overflow-visible">Tailored to your needs.</h2>
      <p class="text-xl ml-1">Showcase your products, market your business, or sell your services.</p>
    </home-section>
    <section id="check-work" class="h-auto min-h-screen w-full flex justify-center items-center">
      <div id="content" class="w-11/12 max-w-4xl flex flex-col justify-center items-center px-8 space-y-8 text-white text-center">
        <h2 class="text-6xl font-medium overflow-visible">Check out our client.</h2>
      <div id="container" class="marker:flex flex-col justify-center items-center space-y-6 md:space-y-0 md:grid md:grid-cols-2 md:grid-flow-row md:gap-8">
        <client/>
        <client/>
        <client/>
        <client/>
      </div>
      <button class="px-4 py-2 border border-white text-lg text-white rounded ease-in duration-200 hover:bg-white hover:text-black">
        <p>More Work</p>
      </button>
      </div>
    </section>
    <home-section>
      <h2 class="text-6xl font-medium overflow-visible">Get involved.</h2>
      <p class="text-xl ml-1">Reach out to us to get started.</p>
      <a id="contact" href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=team@webrising.org" target="_blank">
        <button class="px-4 py-2 border border-white text-lg text-white rounded ease-in duration-200 hover:bg-white hover:text-black">
          <p>Contact Us</p>
        </button>
      </a>
    </home-section>
  </div>
</template>

<script>
import BIRDS from 'vanta/dist/vanta.birds.min'
import gsap from 'gsap'
import ScrollTrigger from 'gsap/ScrollTrigger'

gsap.registerPlugin(ScrollTrigger)

console.log(ScrollTrigger)

export default {
  name: 'Home',
  data() {
    return {}
  },
  mounted() {
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
