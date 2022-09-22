<template>
  
  <main>
    
  </main>
</template>

<script>
export default {
    name: 'resources',
    data (){
      return{
             
        }
    },
    mounted(){
    this.fetchAllProducts()
    },
    methods:{
      async fetchAllProducts(){
        const res=await fetch("https://dummyjson.com/products")
        const json=await res.json()
        console.log(json);

      }
    }

}
</script>

<style>

</style>