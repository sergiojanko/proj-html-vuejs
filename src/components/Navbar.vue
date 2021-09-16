<template>
  <div class="navbar">
    <a class="navbar-brand" href="#">
        <img src="@/assets/images/logo_seo_w_1x.png" alt="AvadaSEO" width="150" class="d-inline-block align-text-top">
    </a>
      <ul class="navbar">
        <li v-for="link in links" :key="link">{{link}}</li>
        <li>
             <button type="button" class="btn">Get in touch Now</button>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
name: "Navbar",
data(){
    return {
        links: ["Home", "Who We Are", "What we do", "Where We Work", "Careers", "News"]
    }
}
}
</script>

<style lang="scss" scoped>
ul li 
{
    list-style-type: none;
}
</style>