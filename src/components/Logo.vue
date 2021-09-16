<template>
  <img :src="`${logo[color]}`" alt="AvadaSEO"/>
</template>

<script>
export default {
name:"Logo",
props: ["color"],
data(){
    return{
        logo: {
            white: "@/assets/images/logo_seo_w_2x.png",
            black: "@/assets/images/logo_seo_2x.png",
            
        }
    }
},
computed: {
getLogoPath(){
    return this.logo[this.color];
}
}
}
</script>

<style lang="scss" scoped>

</style>