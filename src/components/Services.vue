<template>
  <section id="services">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h2>See Our Top Notch Services</h2>
        </div>
        <div class="col-12 text-center">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi totam deleniti eaque adipisci eum possimus dicta in quidem. Totam, nemo necessitatibus nulla eius deserunt blanditiis error voluptates facilis nihil veniam.</p>
        </div>
      </div>
      <div class="row">
        <div v-for="(card, i) in cards" :key="i" class="col-3">
          <div class="card">
            <Card :title="card.title" :icon="card.icon" :text="card.text"/>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Card from "@/components/Card.vue"

export default {
name: "Services",
components: {
  Card,
},
data(){
  return {
    cards: [
      {
        icon: "fab fa-google",
        title: "Google SEO",
        text: "lorem ipsum dolor",
      },
      {
        icon: "fas fa-cog",
        title: "Brand strategy",
        text: "lorem ipsum dolor",
      },
      {
        icon: "fas fa-building",
        title: "Local SEO",
        text: "lorem ipsum dolor",
      },
      {
        icon: "fas fa-chart-bar",
        title: "SEO Analysis",
        text: "lorem ipsum dolor",
      },
    ],
  }
}
}
</script>

<style>

</style>