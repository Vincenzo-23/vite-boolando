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

        <div class="col-3" v-for="(product,i) in store.products" :key="product.id" >

          <CardComponent :card="product" :badge="product.badges"/>

        </div>

      </div>


    </div>

  </section>



</main>

</template>


<style lang="scss" scoped>

.col-3{
    width: calc(3 * 100% / 12);
    min-height: 100%;
    
}

.container {
    .row {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 16px;
    }
}



</style>