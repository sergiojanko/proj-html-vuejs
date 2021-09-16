<template>
  <div class="navbar">
      <ul class="navbar">
          <li v-for="link in links" :key="link">{{link}}</li>
      </ul>
      <button>Get in touch Now</button>
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