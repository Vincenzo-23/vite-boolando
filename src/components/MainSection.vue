<script>
import CardComponent from "./CardComponent.vue"
import { store } from "/store.js"

export default {
  components:{
    CardComponent,
  },
  data() {
    return{
      store
    }
  }
}

</script>


<template>

<main>


  <section class="section">

    <!-- Sezione con le card dei prodotti -->

    <div class="container">

      <div class="row">

        <CardComponent />

      </div>


    </div>

  </section>



</main>

</template>


<style lang="scss" scoped>



.container {
    .row {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 16px;
    }
}



</style>