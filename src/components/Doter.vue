<template>	

	<!-- <input  type="text" v-model='goos' > -->

  <mycheckbox @noong='tot' :dpp='foo'></mycheckbox>


</template>

<script>
export default {

  name: 'Doter',

  props:{
    goos:{
      type:String
    },
    fill:{
      type:String
    },
    foo:{
      type:Array
    }
  },
  data () {
    return {
    	goos:'',
      goo:[]

    }
  },
  methods:{
    tot(top){
      console.log(top)

    }
  },
  computed:{
  	lord(){

  	}
  }
}
</script>

<style lang="css" scoped>
.checkbox{
  display :'block'
}
</style>
