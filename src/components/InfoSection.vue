<template>
    <section id="info-section">
        <div class="container">
            <div class="row">
                <h2>Meet The New Agency SEO Templt FromTh Avada Team</h2>
            </div>
            <div class="row">
                <div class="col">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Odio, molestiae eligendi temporibus delectus non cupiditate eius, numquam esse nisi necessitatibus quo laborum quasi commodi, placeat assumenda voluptatibus quos quod blanditiis.</p>
                </div>
            </div>
            <div class="row">
                <div v-for="(card, index) in cards" :key="index" class="col-4">
                    <Card :title="card.title" :text="card.text" :icon="card.icon"/>
                </div>
            </div>
            <div class="row mx-auto">
                <div class="col px-auto">
                    <img src="@/assets/images/agency-seo-desk-front-600x285.jpg" alt="item" class="mx-auto">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Card from "@/components/Card.vue"

export default {
name: "InfoSection",
components: {
    Card,
},
data(){
    return {
        cards: [
            {
                icon: "fas fa-road",
                title: "Establish Goals",
                text: "lorem ipsum dolor",
            },
            {
                icon: "fas fa-video",
                title: "Work With a Team",
                text: "lorem ipsum dolor",
            },
            {
                icon: "fas fa-tint",
                title: "Get Results",
                text: "lorem ipsum dolor",
            },
        ],
    }
}
}
</script>

<style lang="scss" scoped>
    #info-section
    {
        background-color: #f8f8f8;
    }
</style>