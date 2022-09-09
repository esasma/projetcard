<script setup lang="ts">
   import card from "../components/card.vue" ;
   import maisons from "../assets/maisons.json";

   const obj={
nom:"test1",
prix:"34",
   };

</script>
<template>
    <card nom="nom de lamaison" :prix="34"/>
    <card v-bind="obj" />
</template>