<template>
    <div class="cxa">
        <div v-if="contador <5">fff {{ nome }}</div>
        <div >num {{ contador }}</div>
        <button @click="incrementa">
            Incrementar
        </button>
       
    </div>
</template>
  
<script>

export default {

    data() {
        return {
            contador: 1,
            nome: "Pablo"
        }
    },
    methods: {
        incrementa() {
            this.contador++;
        }
    },
}
</script>
<style>
.cxa {
    border: 2px solid black;
    padding: 2px;
    margin: 2px;
}
</style>