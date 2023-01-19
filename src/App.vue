<script>
import AppTitle from './components/AppTitle.vue';
import AppHero from './components/AppHero.vue';
import AppGallery from './components/AppGallery.vue';


export default {
  name:'Homepage',
  data() {
    
  },
  components: {
    AppTitle,
    AppHero,
    AppGallery

  }
}
</script>


<template>
<app-title></app-title>
<app-hero></app-hero>
<app-gallery></app-gallery>
</template>

<style>

</style>