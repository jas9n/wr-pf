<template>
  <div id="projects">
    <global-navbar />
    <section class="min-h-screen w-full justify-center items-center pt-28 pb-12 px-12 space-y-8">
      <h2 class="text-white text-5xl text-center font-medium overflow-visible">Our clients.</h2>
      <div id="container" class="w-full overflow-visible flex flex-row flex-wrap justify-center items-center gap-6">
        <client-profile v-for="client in clients" :key="client.name" :name="client.name" :details="client.details" :image="client.image" />
      </div>
    </section>
    <global-footer />
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data() {
    return {
      clients: [
        {
          name: 'K-Spirit Taekwondo',
          details: 'A Brooklyn Taekwondo Studio',
          image: 'tkd.jpg',
        },
        {
          name: 'Ready, Set, Spike!',
          details: 'NYC-based Volleyball Nonprofit',
          image: 'rss.jpg',
        },
      ],
    }
  },
}
</script>