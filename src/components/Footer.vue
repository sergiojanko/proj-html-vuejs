<template>
  <footer class="text-center">
    <img src="@/assets/images/logo_seo_1x.png" alt="AvadaSEO" width="150">
    <ul class="d-flex justify-content-center">
      <li v-for="link in links" :key="link">{{link}}</li>
    </ul>
    <p>&copy; Copyright 2012-2020 | Avada Theme by ThemeFusion | Powered by Boolean</p>
    <ul class="socials d-flex justify-content-center">
      <li v-for="social in socials" :key="social"><i class="fab" :class="social"></i></li>
    </ul>
  </footer>
</template>

<script>
export default {
name: "Footer",
data(){
  return {
    links: ["Home","Who We Are","What We Do","Where We Work","Careers","News","Get in touch Now"],
    socials: ["fa-facebook-f", "fa-instagram","fa-twitter","fa-youtube"]
  }
}
}
</script>

<style scoped lang="scss">
li
{
  list-style-type: none;
}
</style>