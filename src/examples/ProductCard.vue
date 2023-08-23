<script lang="ts">
import type { Product } from './Product';
export default {
    props: {
        product: {
            type: Object as PropType<Product>,
            required: true
        }
    },
    emits:['addProduct'],
    methods: {
        onAddButtonClick() {
            // console.log('Agregando producto: ' + this.product.id);
            this.$emit('addProduct');

        }
    },
}
</script>



<template>
    <p>Nombre: {{ product.name }} </p>
    <p>Price: ($ {{ product.price }}) </p>
    <button @click="onAddButtonClick">Agregar al carrito</button>
    <hr />

</template>