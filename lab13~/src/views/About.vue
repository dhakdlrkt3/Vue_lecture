<template>
  <div class="about">
    <h1>This is an about page</h1>
      <KossieCoder>
        <!-- v-slot: 은 #으로 축약 가능 -->
          <!-- 
            이렇게 해도 됨
            <template #header="props">
            <p>header111 {{ props.kossie}}</p> -->
          <template #header="{kossie}">
            <p>header111 {{ kossie }}</p>
          </template>
          <template #default>
            hello1
          </template>
      </KossieCoder>
  </div>
</template>
<script>
  import KossieCoder from '@/components/KossieCoder.vue';
  export default {
    components:{
      KossieCoder
    },
    data(){
      return{
        title: 5
      }
    }
  }
</script>