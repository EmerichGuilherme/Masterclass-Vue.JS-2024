<template>
    <div class="componente">
        <h1>
            Componente com dados Reativos Não Primitivos
        </h1>
        <p>Nome: {{ pessoa.nome }} | Idade: {{ pessoa.idade }}</p>
        <button v-on:click="fazerAniversario()">Fazer Aniversário</button>
        <button @click="mudarNome()">Mudar Nome</button>
    </div>
</template>

<!-- <script setup>
//composition API
import {reactive} from "vue"

const pessoa = reactive({nome:'Gui', idade:24})


function fazerAniversario() {
    pessoa.idade +=1
}

function mudarNome() {
    pessoa.nome = "Ana Maria"
}
</script> -->

<script>
//option API
export default {
    data:function() {
        return {
            pessoa: {
                nome: "Gui",
                idade: 24
            }
        }
    },
    methods:{
        fazerAniversario: function(){
            this.pessoa.idade +=1
        },
        mudarNome: function() {
            this.pessoa.nome = "Ana maria"
        }
    }
}
</script>