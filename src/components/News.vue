<template>
  <section id="news">
    <div class="container text-center">
      <div class="row">
        <div class="col-12">
          <h2>Our News</h2>
        </div>
        <div class="col-12">
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima iusto odit quaerat error, facilis odio aliquam cumque est fugit sint delectus corrupti, adipisci ut impedit praesentium tempore vero non nobis?</p>
        </div>
        <div v-for="(card, i) in cards" :key="i" class="col-4">
          <div class="card" style="width: 18rem;">
            <img :src="getImageUrl(card.img)" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">{{card.title}}</h5>
              <p class="card-subtitle">{{card.subtitle}}</p>
              <p class="card-text">{{card.text}}</p>
            </div>
          </div>
        </div>
        <div class="col-12">
          <button type="button" class="btn btn-prim"> GO TO NEWS</button>
        </div>
      </div>
    </div>
    
  </section>
</template>

<script>
export default {
name: "News",
data(){
  return {
    cards:[
      {
        img: "blog-post-6-320x202.jpg",
        title: "Why You Need a SEO Agency Now",
        subtitle: "November 1st, 2017",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, provident iusto aspernatur in qui eveniet adipisci architecto quae, ratione iure perspiciatis? Pariatur sed cupiditate incidunt hic provident porro possimus necessitatibus?"
      },
      {
        img: "related-service-2-320x202.jpg",
        title: "SEO Tips For Your Startup",
        subtitle: "November 1st, 2017",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, provident iusto aspernatur in qui eveniet adipisci architecto quae, ratione iure perspiciatis? Pariatur sed cupiditate incidunt hic provident porro possimus necessitatibus?"
      },
      {
        img: "related-service-4-320x202.jpg",
        title: "Image Optimization For Your Site",
        subtitle: "November 1st, 2017",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, provident iusto aspernatur in qui eveniet adipisci architecto quae, ratione iure perspiciatis? Pariatur sed cupiditate incidunt hic provident porro possimus necessitatibus?"
      },
    ],
  }
  },
methods: {
  getImageUrl(img){
    return require("../assets/images/" + img);
  },
}
}
</script>

<style>

</style>