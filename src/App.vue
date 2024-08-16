<script setup>
import primeiroComponente from './components/primeiroComponente.vue';
import comDados from './components/comDados.vue'
import comDadosReativosPrimitivos from './components/comDadosReativosPrimitivos.vue'
import comDadosReativosNaoPrimitivos from './components/comDadosReativosNaoPrimitivos.vue';
import dataBinding from './components/dataBinding.vue';
import comProps from './components/comProps.vue';
</script>

<template>
    <header>Vue</header>
    <comProps item="Borracha" :preco="2.50"/>
    <dataBinding/>
    <comDadosReativosNaoPrimitivos/>
    <comDadosReativosPrimitivos/>
    <comDados/>
    <primeiroComponente/>
</template>

