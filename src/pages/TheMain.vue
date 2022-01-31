<template>
  <main class="flex flex-col">
    <div class="flex justify-between px-10 py-6 items-center">
      <InputComponent />
      <SelectComponent
        :selected="filter"
        @update:selected="onChange"
      />
    </div>
  </main>
</template>

<script>
    import InputComponent from '../components/ui/InputComponent.vue'
    import SelectComponent from '../components/ui/SelectComponent.vue'

export default {
    name:'TheMain',
    components:{InputComponent, SelectComponent},
    data(){
      return{
        filter:''
      }
    },
    methods:{
      onChange(value){
        this.filter = value
      }
    }
  }
</script>

<style>

</style>