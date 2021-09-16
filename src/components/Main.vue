<template>
  <main>
    <InfoSection/>
    <Services/>
    <Work/>
    <Plans/>
    <News/>
    <Partners/>
    <Contact/>
  </main>
</template>


<script>
import InfoSection from "@/components/InfoSection.vue"

export default {
name: "Main",
components: {
  InfoSection,
  Services,
  Work,
  Plans,
  News,
  Partners,
  Contact,
}
}
</script>

<style lang="scss" scoped>

</style>