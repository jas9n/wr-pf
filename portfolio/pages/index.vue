<template>
  <div id="home">
    <navbar/>
    <div id="birds" class="bg-black h-screen" ref="birdsRef">

    </div>
    <div id="splash" class="bg-white h-screen">

    </div>
  </div>
</template>

<script>
import BIRDS from "vanta/src/vanta.birds";
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";

gsap.registerPlugin(ScrollTrigger);

console.log(ScrollTrigger);

export default {
  name: 'Home',
  data() {
    return {

    }
  },
  mounted() {
    this.vantaEffect = BIRDS({
      el: this.$refs.birdsRef,
      mouseControls: false,
      touchControls: false,
      gyroControls: false,
      maxHeight: 200.0,
      maxWidth: 200.0,
      scale: 1.0,
      scaleMobile: 1.0,
      backgroundColor: 0x151515,
      color1: 0xb11e1e,
      color2: 0x217c91,
      birdSize: 1.2,
      wingSpan: 20.0,
      speedLimit: 3.0,
      quantity: 4.0,
    });
  }
}
</script>
