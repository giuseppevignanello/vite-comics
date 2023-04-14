<script>
import topFooter from "./Footer/topFooter.vue"
import bottomFooter from "./Footer/bottomFooter.vue"
export default {
  name: "appFooter",
  components: {
    topFooter,
    bottomFooter
  },
  data() {
    return {  
    }
  }
}
</script>

<template>
  <footer>
   <topFooter/>
   <bottomFooter/>
  </footer>
</template> 