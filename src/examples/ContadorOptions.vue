<!-- Este ejemplo esta escrito utilizando VUE (Options API) usado sobre todo en vue2 (por eso la etiqueta <script> no tiene <sript setup>)-->

<script lang="ts">
export default {
    data() {
        return {
            count: 0
        };
    },

    methods: {
        increase() {
            this.count += 1;
        },
        decrease() {
            this.count -= 1;
        }
    },
    mounted() {
        console.log("el valor inicial del contador es:" + this.count);
    }
};
</script>

<template>
    <h1>contador: {{ count }} </h1>
        <button @click="decrease">Reducir contador</button>
        <button @click="increase">Aumentar contador</button>
    <p>(Version Options API)</p>



    <!-- <button @click="count = count-1">Reducir contador</button> -->
</template>

