<template>
  <div id="projects">
    <global-navbar />
    <section class="min-h-screen w-full justify-center items-center pt-32 pb-12 px-12">
      <h2 class="w-3/4 text-white text-5xl text-center font-medium overflow-visible">Our clients.</h2>
      <div id="container" class="w-full overflow-visible grid grid-cols-1 grid-flow-row justify-items-center place-content-center gap-2 md:grid-cols-2 lg:grid-cols-3">
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