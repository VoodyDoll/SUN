<template>	

	<input  type="text" v-model='goos'>
	<!-- <button @click='lord' >Ok</button> -->


</template>

<script>
export default {

  name: 'Doter',
  
props:{
  goos:{
    type:String
  }
},
  data () {
    return {
    	goos:'',
      goo:[]

    }
  },
  methods:{
    foomo(){
      
      // console.log(this.goo)
    }
  },
  computed:{
  	lord(){
      this.goo.push(this.goos)
  		console.log(this.goo)
  	}
  }
}
</script>

<style lang="css" scoped>
</style>
