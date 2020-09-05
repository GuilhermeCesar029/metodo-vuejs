<template>
    <div class="metodo">
        <label>Qual seu nome?</label><br>
        <input v-model="nomeField" placeholder="Seu nome"><br>
        <button v-on:click="cumprimentar">Cumprimentar</button>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                nomeField: "",
            }            
        },
        methods: {
            cumprimentar: function() {
                alert('olá ' + this.nomeField + '!')
            }
        }
    }
</script>

<style scoped>
    .metodo {
        text-align: center;
    }
</style>