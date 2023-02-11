

<template>

  <div class="flex justify-center">
    <div class="bg-white w-8/12 flex-column text-center">
      <h1 class="pt-5 text-blue-600 font-medium">Inizia la tua ricerca di un immobile all'asta</h1>
      <div class="flex-column p-2 ">
        <!-- <p>Questa casa si trova : {{ locazione }}</p> -->
        <Input v-model="locazione" placeholder="Inserisci comune o provincia" />
        <DropDown filterPlaceHolder="Destinazione immobile" />
        <DropDown filterPlaceHolder="Tipologia immobile" />
      </div>

      <Bottone functionality="Cerca" bgColor="bg-blue-500" />

    </div>
  </div>
</template>

<script>



import Input from './partials/Input.vue';
import DropDown from './partials/DropDown.vue';
import Bottone from './partials/Bottone.vue';

export default {


  /*  data() {
     return {
       locazione: ""
     }
   }, */


  name: "HouseForm",


  components: {

    Input,
    DropDown,
    Bottone
  }
}
</script>