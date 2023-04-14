<script>
import comicsList from "./Main/comicsList.vue"
import banner from "./Main/appBanner.vue"
export default {
  name: "appMain",
  components: {
    comicsList, 
    banner
  },
  data() {
    return {
    }
  }, 
}
</script>

<template>
  <main>
   <comicsList/>
   <banner/>
   
  </main>
</template> 

<style scoped lang="scss"></style>