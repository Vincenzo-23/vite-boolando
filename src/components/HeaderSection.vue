<script>
export default {
  data() {
    return {
      models: ["Donna", "Uomo", "Bambini"],
    } 
  }
}
</script>


<template>
  
  <header>
    <div class="container-header">
      <div class="row">
        <ul class="col-3-header">
          <li v-for="(model, i) in models"><a href="#">{{ models[i] }}</a></li>
        </ul>
        <div class="col-6-header">
          <img class="logo" src="/boolean-logo.png" alt="Logo Boolean">
        </div>
        <ul class="col-3-header">
          <li><a href="#">&hearts;</a></li>
          <li><a href="#">&star;</a></li>
          <li><a href="#">&circledR;</a></li>
        </ul>
      </div>
    </div>
  </header>
  
</template>


<style lang="scss" scoped>

.container-header{
  max-width: 2048px;
  margin: 0 auto;
  padding: 0 20px;
  .row {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    gap: 50px;
  }
}



.col-3-header{
  font-size: 20px;
  display: flex;
  gap: 15px;
  align-items: center;
}


.logo{
  width: 150px;
}


header{
  padding: 20px 0;
  color: white;
  margin-bottom: 50px;
  background-color: rgb(255, 105, 0);

}

</style>