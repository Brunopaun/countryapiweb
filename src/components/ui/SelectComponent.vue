<template>
  <select
    :value="selected"
    @change="$emit('update:selected', $event.target.value)"
  >
    <option
      disabled
      value=""
    >
      Filter by Region
    </option>
    <option
      v-for="cont in continent"
      :key="cont"
      :value="cont"
    >
      {{ cont }}
    </option>
  </select>
</template>

<script>
export default {
    name:'SelectComponent',
    props:{
      selected:{
      type:String,
      default:''
    }},
    emits:['update:selected'],
    data(){
      return {
        continent: ['Africa', 'Americas','Asia','Europe','Oceania'],
      }
    },
}
</script>

<style>

</style>