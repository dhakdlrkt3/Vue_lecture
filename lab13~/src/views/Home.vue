<template>
  <div>
    <h1>This is home page</h1>
    <form action="">
        <InputField v-model="name"/>
      <br>
      <button>Submit</button>
    </form>
    {{ name }}
  </div>
</template>

<script>
import InputField from '@/components/InputField.vue';
export default {
  components:{
    InputField
  },
  data(){
    return{
      name:'Kossie Coder'
    }
  },

  beforeCreate(){
    console.log('beforeCreate', this.name)
  },
  created(){
    
  },
  beforeMount(){
    
  },
  mounted(){

  },
  beforeUpdate(){
    
    
  },
  updated(){

  },
  destroyed(){

  }



}
</script>

<style scoped>
h1{
  color: red;
}
</style>