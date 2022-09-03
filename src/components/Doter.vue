<template>	

	<input @input='lord' type="text" v-model='goos'>
	<button >Ok</button>


</template>

<script>
export default {

  name: 'Doter',

  data () {
    return {
    	goos:''

    }
  },
  methods:{

  },
  computed:{
  	lord(Value){
  		console.log(Value.goos)
  	}
  }
}
</script>

<style lang="css" scoped>
</style>
