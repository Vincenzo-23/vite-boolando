<script>
export default {
  data() {

  }
}
</script>


<template>
  
  <header>
    <div class="container-header">
      <div class="row">
        <div class="col-3-header">
          <a href="#">Donna</a>
          <a href="#">Uomo</a>
          <a href="#">Bambini</a>
        </div>
        <div class="col-6-header">
          <img class="logo" src="/boolean-logo.png" alt="Logo Boolean">
        </div>
        <div class="col-3-header">
          <a href="">&hearts;</a>
          <a href="">&star;</a>
          <a href="">&circledR;</a>
        </div>
      </div>
    </div>
  </header>
  
</template>


<style lang="scss" scoped>

.container-header{
    max-width: 2048px;
    margin: 0 auto;
    padding: 0 20px;
}



.container-header .row {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    gap: 50px;
}


.col-3-header{
    font-size: 20px;
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