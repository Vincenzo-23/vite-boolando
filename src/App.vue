<script>
import HeaderSection from "./components/HeaderSection.vue"
import MainSection from "./components/MainSection.vue"
import FooterSection from "./components/FooterSection.vue"
import { store } from "/store.js"
import axios from "axios"

export default {
  data(){
    return{
      
    }
  },
  components:{
    HeaderSection,
    MainSection,
    FooterSection
  },
  methods: {
    fetchProducts(){
      axios.get("http://localhost:3000/products").then((res) => {
        store.products = res.data
      })
    }
  },
  created(){
    this.fetchProducts()
  }
}
</script>

<template>
  <HeaderSection/>
  <MainSection/>
  <FooterSection/>
</template>

<style lang="scss">

@use "./style/general";

</style>