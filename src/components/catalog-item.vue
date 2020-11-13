<template>
    <div class="catalog-item" v-for="product in products" :key="product.id" @mouseover="showButton">
        <img :src="product.image">
        <p>{{ title }}</p>
        <div class="catalog-item-func">
            <p>{{ product.price }}</p>
            <button @click="addToCart">+</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'catalog-item',
        data() {
            return {
            category: 'Краска',
            brand: 'Wallquest',
            model: 'Brownsone MS90102',
            cart: 0,
            products: [
                    { image: '../assets/images/1.png', price: 6000, id: '1' },
                    { image: './assets/images/2.png', price: 4800, id: '2' },
                    { image: './assets/images/3.png', price: 5290, id: '3' },
                    { image: './assets/images/4.png', price: 2800, id: '4' },
                    { image: './assets/images/5.png', price: 3400, id: '5' },
                    { image: './assets/images/6.png', price: 6000, id: '6' },
                    { image: './assets/images/7.png', price: 4800, id: '7' },
                    { image: './assets/images/7.png', price: 5290, id: '8' },
                    { image: './assets/images/8.png', price: 2800, id: '9' },
                    { image: './assets/images/9.png', price: 3400, id: '10' },
                    { image: './assets/images/6.png', price: 6000, id: '11' },
                    { image: './assets/images/7.png', price: 4800, id: '12' },
                    { image: './assets/images/7.png', price: 5290, id: '13' },
                    { image: './assets/images/8.png', price: 2800, id: '14' },
                    { image: './assets/images/9.png', price: 3400, id: '15' },
                ],
            }
        },
        methods: {
            addToCart() {
                this.cart += 1
            },
            showButton() {
                return 
            }
        },
        computed: {
            title() {
                return this.category + ' ' + this.brand + ', ' + this.model
            }
        }
    }
</script>

<style scoped>
    .catalog-item {
        display: flex;
        flex-direction: column;
        border-bottom: 1px solid #000;
    }
    .catalog-item-func {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }
</style>