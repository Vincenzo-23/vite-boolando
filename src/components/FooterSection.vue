<script>
export default {
  data() {

  }
}
</script>


<template>

    <footer>
        <div class="container">
            <div class="row-footer">
                <div class="col-10">
                    <h3>Boolando s.r.l</h3>
                    <div>
                        <a href="#">Informazioni legali</a>
                        <a href="#">Informativa sulla privacy</a>
                        <a href="#">Diritto di recesso</a>
                    </div>
                </div>
                <div class="col-2">
                    <div>Trovaci anche su</div>
                    <div>
                        <a href="#">Fb</a>
                        <a href="#">YT</a>
                        <a href="#">Ig</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>


<style lang="scss" scoped>

footer{
    background-color: rgb(26, 26, 26);
    color: white; 
    padding-top: 15px;
    padding-bottom: 10px;
    margin-top: 50px;
}


.container{
    .row-footer{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    gap: 16px;
    height: 50px;
    }
}

</style>