<!-- Este ejemplo esta escrito utilizando VUE Compositions API etiqueta <script> tiene <sript setup>-->
<script setup lang="ts">
    import { onMounted, ref } from 'vue';

    const count = ref (0);

    function aumentar(){
        count.value += 1;
    };
    function reducir(){
        count.value -= 1;
    };
    onMounted(() => {
        console.log("El valor inicial del contador es: " + count.value);
    });

</script>

<template>
    <p>Version Compositions API</p>

    <h1>Contador: {{ count }} </h1>

    <button @click="reducir" >Reducir Contador</button>
    <button @click="aumentar" >Incrmentar Contador</button>


</template>

