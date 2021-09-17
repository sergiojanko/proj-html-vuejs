<template>
  <section id="partners">
    <div class="container text-center">
      <div class="row">
        <div class="col-12">
          <h2>What Our Clients Say</h2>
        </div>
        <div class="col-12">
          <div v-for="(partner, i) in partners" :key="i" class="partners" :class="partner.active ? 'active':'d-none'">
            <img :src="getImageUrl(partner.img)" alt="">
            <p class="partner-text">{{partner.text}}</p>
            <p class="partner-name">{{partner.name}}</p>
          </div>
        </div>
        <hr>
        <div v-for="logo in logos" :key="logo" class="col-3">
          <div class="partner-logo"><img :src="getImageUrl(logo)" alt=""></div>
        </div>
      </div>
      
    </div>
  </section>
</template>

<script>
export default {
name:"Partners",
data(){
  return{
    partners: [
      {
        img: "testimonials-2.jpg",
        text: "Ability proceeds from a fusion of skills, knowledge, understanding and imagination",
        name: "Luis Desalvo",
        active: true,
      },
      {
        img: "testimonials-1.jpg",
        text: "Ability proceeds from a fusion of skills, knowledge, understanding and imagination",
        name: "Luisa Salvode",
        active: false,
      },
    ],
    logos: ["clients_partner_1-200x202.png","clients_partner_2-200x202.png","clients_partner_3-200x202.png","clients_partner_4-200x202.png"],
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
.partners img 
{
  border-radius: 50%;
}
</style>