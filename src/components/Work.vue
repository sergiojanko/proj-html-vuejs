<template>
  <section id="work" class="text-center">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h2>Our Work</h2>
        </div>
        <div class="col-12 d-flex justify-content-center">
          <p class="w-50">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sunt vero debitis dolorum nostrum, iusto id numquam quibusdam quod error aperiam! Incidunt, quasi hic ratione minus ipsam quaerat exercitationem harum dolores?</p>
        </div>
        <div v-for="img in images" :key="img"  class="col-4 p-2">
          <img :src="getImageUrl(img)" alt="case study" class="m-2">
        </div>
        <div class="col">
          <button type="button" class="btn btn-prim mt-2 mb-5">VIEW OUR WORK</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
name: "Work",
data(){
  return {
    images: [
      "case-study-gallery-1-1-600x450.jpg",
      "case-study-gallery-2-600x450.jpg",
      "case-study-gallery-3-1-600x450.jpg",
      "case-study-gallery-4-1-600x450.jpg",
      "case-study-gallery-5-1-600x450.jpg",
      "case-study-gallery-6-1-600x450.jpg",

      ]
  }
},
methods: {
      getImageUrl(img){
        return require("../assets/images/" + img);
      },
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables";

img
{
  max-width: 300px;
}

#work
{
  background-color: $light-gray;
}
</style>
