<template>
<!-- <div v-for="item in dpp" class="checkbox" >	    
      <input  type="checkbox" value='item.age' @change='loozo' id='item.age'>
    <label :for="item.name">
     {{item.name}}
    </label>      
  
</div> -->
 <input  type="checkbox" value='item.tgf'  id='poop' v-model='carl'>
    <label for="poop">Пальма</label>
      
     <input  type="checkbox" value='item.fd'  id='zooz' v-model='carl'>
    <label for="zooz">Веды</label>
  
     <input  type="checkbox" value='item.agdfge'  id='citty' v-model='carl'>
    <label for="citty">Закон</label>
   <!-- <p>{{carl}}</p> -->
     <button @click='loozo'>Ok</button>
</template>

<script>
export default {

  name: 'Mycheckbox',
  props:{
  	dpp:{
  		type:[String,Array]
  	}
  },

  data () {
    return {
      carl:[]

    }
  },
  methods:{    
    loozo(){
      this.$emit('noong',this.carl)
    }
  },
  // watch:{
  //   carl(er){
  //     this.$emit('noong',er)
  //     // console.log(er)
  //   }
  // }
}
</script>

<style lang="css" scoped>
</style>