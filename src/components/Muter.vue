<template>
<doter :foo='faza'></doter>
	<input type="text" :value='got'>

</template>

<script>
import Doter from '@/components/Doter.vue'

export default {
components:{
   Doter
  },
  name: 'Muter',

  data () {
    return {
      got:'',
      faza:[
      {valuess:'focuss',name:'Фикус'},
      {valuess:'loid',name:'Пальма'},
      {valuess:'chankala',name:'Хвощ'},
      {valuess:'zizan',name:'Пудра'}

      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
