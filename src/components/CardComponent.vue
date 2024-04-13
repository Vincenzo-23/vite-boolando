<script>
import { store } from "/store.js"

export default {
    data() {
        return{
            store
        }
    }
}
</script>


<template>
    <div class="col-3" v-for="(product,i) in store.products" :key="product.id" >
        <div class="card">
            <div class="card-header">
                <img :src="store.products[i].frontImage" alt="Picture of a model with the white shirt and beige pants">
                <img class="hover-img" :src="store.products[i].backImage" alt="Picture of a model with the white shirt and beige pants with a brown jacket">
                <ul class="badge-container">
                    <li v-for="(badge,i) in store.products[i].badges" :key="i" 
                    :class="`badge_${badge.type}`">{{ badge.value }}</li>
                </ul>
                <button class="like-button">&hearts;</button>
            </div>
            <div class="card-footer">
                <div class="card-footer-brand" >{{ store.products[i].brand }}</div>
                <h3 class="card-footer-title">{{ store.products[i].name }}</h3>
                <div class="card-footer-price">{{ store.products[i].price }} €</div>
            </div>
        </div>
    </div>

</template>


<style lang="scss" scoped>

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
    display: flex;
    gap: 10px;
}

 .badge_discount{
    background-color: red;
    padding: 5px 5px;
    order: -1;
    
}

.badge_tag{
   
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