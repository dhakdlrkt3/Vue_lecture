<template>
  <div>
    <h1>This is home page</h1>
    <!-- <KossieCoder title="home title" name="코지 코더"/> -->
    <form>
  </div>
</template>

<script>
import KossieCoder from '@/components/KossieCoder.vue';
export default {
  components: {
    KossieCoder
  },
  data(){
    return{
      name: 'Kossie Coder'
    }
  }
}
</script>

<style scoped>
h1{
  color: red;
}
</style>