<template>
  <main>
    <InfoSection/>
    <Services/>
    <Work/>
    <Plans/>
    <News/>
    <Partners/>
    <Contacts/>
  </main>
</template>


<script>
import InfoSection from "@/components/InfoSection.vue"
import Services from "@/components/Services.vue"
import Work from "@/components/Work.vue"
import Plans from "@/components/Plans.vue"
import News from "@/components/News.vue"
import Partners from "@/components/Partners.vue"
import Contacts from "@/components/Contacts.vue"

export default {
name: "Main",
components: {
  InfoSection,
  Services,
  Work,
  Plans,
  News,
  Partners,
  Contacts,
}
}
</script>

<style lang="scss" scoped>

</style>