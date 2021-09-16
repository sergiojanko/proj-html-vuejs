<template>
  <header>
      <div class="container">
          <div class="row">
              <div class="col-4">
                  <Logo color="white"/>
              </div>
              <div class="col-8">
                  <Navbar/>
              </div>
          </div>
          <div class="row">
              <div class="col">
                  <HeroContent/>
              </div>
          </div>
      </div>
  </header>
</template>

<script>


import Logo from '@/components/Logo.vue';
import Navbar from '@/components/Navbar.vue';
import HeroContent from '@/components/HeroContent.vue';

export default {
name: "Header",
components: {
    Logo,
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
    background-size: contain;
    height: 800px;
}
</style>