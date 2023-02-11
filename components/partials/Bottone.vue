<template>

  <button :class="{
    [bgColor]: true,
    [fontColor]: true,
    'text-white': !fontColor,
  }" class="font-bold w-9/12 py-4 rounded-3xl mb-7">{{ functionality }}</button>

</template>

<script>

export default {

  name: "Bottone",

  props: {
    functionality: String,
    bgColor: String,
    fontColor: String,
  }
}


</script>