<script>
export default {
  data() {
    return{
        
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

                <div class="col-3">
                    <div class="card-header">
                        <img src="/1.webp" alt="Picture of a model with the white shirt and beige pants">
                        <img class="hover-img" src="/1b.webp" alt="Picture of a model with the white shirt and beige pants with a brown jacket">
                        <div class="badge-container">
                            <span class="discount-badge">-50%</span>
                            <span class="sustainability">Sostenibilità</span>
                        </div>
                        <button class="like-button">&hearts;</button>
                    </div>
                    <div class="card-footer">
                        <div class="card-footer-brand">Levi's</div>
                        <h3 class="card-footer-title">RELAXED FIT TEE UNISEX</h3>
                        <div class="card-footer-price">14,99 € 
                            <span class="old-price">29,99 €</span>
                        </div>
                    </div>
                </div>

                <div class="col-3">
                    <div class="card-header">
                        <img src="/2.webp" alt="Picture of a model with the red and white skirt">
                        <img class="hover-img" src="/2b.webp" alt="Picture of a model with the red and white skirt from a different angle">
                        <div class="badge-container">
                            <span class="discount-badge">-30%</span>
                        </div>    
                        <button class="like-button">&hearts;</button>
                    </div>
                    <div class="card-footer">
                        <div class="card-footer-brand">Guess</div>
                        <h3 class="card-footer-title">ROSES TEE</h3>
                        <div class="card-footer-price">20,99 € 
                            <span class="old-price">29,99 €</span>
                        </div>
                    </div>
                </div>

                <div class="col-3">
                    <div class="card-header">
                        <img src="/3.webp" alt="Picture of a model with the green suit">
                        <img class="hover-img" src="/3b.webp" alt="Picture of a model with the beige suit">
                        <div class="badge-container">
                            <span class="discount-badge">-30%</span>
                        </div>    
                        <button class="like-button">&hearts;</button>
                    </div>
                    <div class="card-footer">
                        <div class="card-footer-brand">Come Zucchero Filato</div>
                        <h3 class="card-footer-title">VOGLIA DI COLORI PASTELLO</h3>
                        <div class="card-footer-price">129,99 € 
                            <span class="old-price">184,99 €</span>
                        </div>
                    </div>
                </div>

                <div class="col-3">
                    <div class="card-header">
                        <img src="/4.webp" alt="Picture of a model with the white shirt and jeans">
                        <img class="hover-img" src="/4b.webp" alt="Picture of a model with the white shirt and jeans from a different angle">
                        <div class="badge-container">
                            <span class="discount-badge">-50%</span>
                            <span class="sustainability">Sostenibilità</span>
                        </div>    
                        <button class="like-button">&hearts;</button>
                    </div>
                    <div class="card-footer">
                        <div class="card-footer-brand">Levi's</div>
                        <h3 class="card-footer-title">TEE UNISEX</h3>
                        <div class="card-footer-price">14,99 € 
                            <span class="old-price">29,99€</span>
                        </div>
                    </div>    
                </div>

                <div class="col-3">
                    <div class="card-header">
                        <img src="/5.webp" alt="Picture of a model with the beige dress">
                        <img class="hover-img" src="/5b.webp" alt="Picture of a model with the beige dress from a different angle">
                        <button class="like-button">&hearts;</button>
                    </div>
                    <div class="card-footer">
                        <div class="card-footer-brand">Maya Deluxe</div>
                        <h3 class="card-footer-title">STRIPE BODICE</h3>
                        <div class="card-footer-price">99,99 €</div>
                    </div>    
                </div>

                <div class="col-3">
                    <div class="card-header">
                        <img src="/6.webp" alt="Picture of a model with the black shirt and brown skirt">
                        <img class="hover-img" src="/6b.webp" alt="Picture of a model with the black shirt and brown skirt from a different angle">
                        <div class="badge-container">
                            <span class="sustainability">Sostenibilità</span>
                        </div>
                        <button class="like-button">&hearts;</button>
                    </div>
                    <div class="card-footer">
                        <div class="card-footer-brand">Esprit</div>
                        <h3 class="card-footer-title">MAGLIONE - BLACK</h3>
                        <div class="card-footer-price">29,99 €</div>
                    </div>
                </div>

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

.col-3{
    width: calc(3 * 100% / 12);
    min-height: 100%;
    
}



/* CARD STYLE */



/* Card Footer */


.card-footer-brand{
    color: rgb(65, 65, 65);
}

.card-footer-title{
    font-size: 14px;
    font-weight: 700;
}

.card-footer-price{
    color: rgb(219, 0, 0);
    font-weight: 700;
}

.old-price{
    color: rgb(65, 65, 65);;
    font-weight: 400;
    text-decoration: line-through;
    
}


    /* Card header */


.card-header{
    position: relative;
}

.badge-container{
    position: absolute;
    bottom: 50px;
    left: 0;
    color: white;
    font-weight: 700;
}

 .discount-badge{
    background-color: red;
    padding: 5px 5px;
    
}

.sustainability{
   
    background-color: green;
    padding: 5px 5px;
}
    

.like-button{
    position: absolute;
    background-color: white;
    padding: 8px 12px;
    font-size: 24px;
    top: 15px;
    right: 0;
}




.hover-img{
    position: absolute;
    left: 0;
    opacity: 0;
    &:hover {
    opacity: 1;
    }
}



</style>