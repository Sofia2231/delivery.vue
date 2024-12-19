

<template>
    <section class="products">
                <div class="products-wrapper" id="food-container">
                        <div class="products-card"
                            v-for="food in foodArray"
                            :key="food.id"
                             >
                            <div class="products-card_image">
                            <img :src="getUrl1(food.image)" alt="food1">
                            </div>
                            <div class="products-card_description">
                            <div class="products-card_description-row">
                             <h5 class="products-card_description-name">
                               {{food.title}}
                             </h5>
                            </div>
                            <div class="products-card_description-row">
                               <p class="products-card_description-text">
                                {{ food.discription }}</p>
                              </div>
                              <div class="products-card_description-row">
                            <div class="products-card_description-controls">
                                <button class="btn btn-primary">
                                    В корзину
                                    <img src="../assets/images/icons/w container.svg" alt="w"/>
                                </button>

                                <span class="products-card_description-controls--price"> {{ food.price }} ₽</span>
                                </div>
                             </div>
                         </div>
                        </div>
                </div>
                        
    </section>
</template>

<script setup>
import { foodArray } from '@/constants/food';
const getUrl1 = (name) => {
    return new URL(`../assets/images/goods/${name}`, import.meta.url)
}


</script>