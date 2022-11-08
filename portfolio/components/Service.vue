<template>
  <div id="service" class="flex flex-col space-y-4">
    <a :href="url" class="w-1/2" target="_blank">
      <img :src="require(`../assets/icons/${logo}`)" class="" alt="" id="pic" />
    </a>
    <h2 class="text-3xl">{{ name }}</h2>
    <ul class="">
      <li class="" v-for="li in description" :key="li">{{ li }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Service',
  props: {
    name: String,
    logo: String,
    url: String,
    description: Array,
  },
}
</script>

<style>
</style>