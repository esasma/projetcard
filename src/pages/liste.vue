<script setup lang="ts">
    import card from "../components/card.vue" ;

    const maisons = [ {nom:"test", prix:24}, { nom:"test2", prix:24 },{ nom:"test3", prix:"24" },{ nom:"test5", prix:"24" }];
    
</script>
<template>
    <div class="p-2">
        <h1 class="text-2xl">Page liste </h1>
        <div v-for="maison in maisons" :key="maison.nom" >
            <card v-bind="maison"/>
        </div>
    </div>
</template>