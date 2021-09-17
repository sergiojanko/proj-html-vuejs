<template>
  <section id="plans" class="text-center">
    <div class="container">
      <div class="row">
        <div class="col-12 text-white">
          <h2>Our Plans</h2>
        </div>
        <div class="col-12 text-white">
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima iusto odit quaerat error, facilis odio aliquam cumque est fugit sint delectus corrupti, adipisci ut impedit praesentium tempore vero non nobis?</p>
        </div>
        <div v-for="(plan, index) in plans" :key="index" class="col-3">
          <div class="plan-card">
            <h3>{{plan.title}}</h3>
            <div class="price">
              {{plan.price}}
            </div>
            <p class="projects">
              {{plan.projects}}
            </p>
            <p class="storage">
              {{plan.storage}}
            </p>
            <p class="users">
              {{plan.users}}
            </p>
            <button type="button" class="btn">START TODAY</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
name: "Plans",
data(){
  return {
    plans: [
      {
        title: "Standard",
        price: "19",
        projects: "5 projects",
        storage: "5 GB Storage",
        users: "Unlimited Users",
      },
      {
        title: "Premium",
        price: "29",
        projects: "10 projects",
        storage: "15 GB Storage",
        users: "Unlimited Users",
      },
      {
        title: "Professional",
        price: "39",
        projects: "15 projects",
        storage: "30 GB Storage",
        users: "Unlimited Users",
      },
      {
        title: "Extreme",
        price: "59",
        projects: "unlimited projects",
        storage: "unlimited GB Storage",
        users: "Unlimited Users",
      },
    ]
  }
}
}
</script>

<style scoped>
#plans
{
  background-image: url("../assets/images/background1.jpg");
  background-size: cover;
}

.plan-card
{
  background-color: #f8f8f8;
}
</style>