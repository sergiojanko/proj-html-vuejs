<template>
  <section id="services">
    <div class="container text-white text-center">
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
            <Card :title="card.title" :icon="card.icon" :text="card.text" :bottomText="'Read More >'"/>
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
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum earum vero eius quas numquam fugit sequi pariatur porro ratione quos ducimus quod id laborum, error quasi non, totam, nihil sunt!",
      },
      {
        icon: "fas fa-cog",
        title: "Brand strategy",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum earum vero eius quas numquam fugit sequi pariatur porro ratione quos ducimus quod id laborum, error quasi non, totam, nihil sunt!",
      },
      {
        icon: "fas fa-building",
        title: "Local SEO",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum earum vero eius quas numquam fugit sequi pariatur porro ratione quos ducimus quod id laborum, error quasi non, totam, nihil sunt!",
      },
      {
        icon: "fas fa-chart-bar",
        title: "SEO Analysis",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum earum vero eius quas numquam fugit sequi pariatur porro ratione quos ducimus quod id laborum, error quasi non, totam, nihil sunt!",
      },
    ],
  }
}
}
</script>

<style lang="scss" scoped>

@import "@/assets/scss/_variables.scss";

#services
{
  background-color: $dark-blue;
  background-image: url("../assets/images/lines-1.png");
  background-size: cover;
  .container{
      background-image: url("../assets/images/pattern_background.png");
      background-size: contain;
      background-repeat: no-repeat;
  }
  .card {
    background-color: $blue;
    border: none;
  }
}
</style>

