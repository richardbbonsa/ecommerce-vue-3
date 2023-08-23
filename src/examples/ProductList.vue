<script lang="ts">
import ProductCard from './ProductCard.vue';

    export default {
    components: { ProductCard},


    data() {
        return {
            products: <Array<Product>> [
                { name: 'Silla', price: 56, id: 5 },
                { name: 'Monitor', price: 450, id: 7 },
                { name: 'Microfono', price:  20, id: 12 }
            ]
        };
    },
    methods: {
        onAddProduct(productId: number) {
            console.log('Agregar Producto ' + productId)
        }
    },
};
    </script>
    
    <template>
    <ProductCard
        v-for="p in products"
        :product="p"
        @addProduct="onAddProduct(p.id)" />
    </template>
    
    
    