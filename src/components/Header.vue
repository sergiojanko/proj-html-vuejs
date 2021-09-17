<template>
  <header class="pb-5">
      <div class="container text-white">
          <div class="row p-2">
              <div class="col">
                  <Navbar/>
              </div>             
          </div>
          <div class="row">
              <div class="col-6">
                  <HeroContent/>
              </div>
          </div>
    </div> 
  </header>
</template>

<script>



import Navbar from '@/components/Navbar.vue';
import HeroContent from '@/components/HeroContent.vue';

export default {
name: "Header",
components: {
    Navbar,
    HeroContent,
},
}
</script>

<style lang="scss" scoped>
header
{
    background-image: url("../assets/images/1-hero-image.png");
    background-position: center;
    background-size: cover;
}
</style>