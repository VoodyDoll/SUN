<template>
	<input type="text" :value='myvalue' @input='horh'>

</template>

<script>
export default {

  name: 'my-input',
  props:{
  	myvalue:{
  		type:[String, Number]
  	}
  },

  data () {
    return {

    }
  },
  methods:{
  	horh(event){
  		this.$emit('update:myvalue',event.target.value)
  	}
  }
}
</script>

<style lang="css" scoped>
</style>