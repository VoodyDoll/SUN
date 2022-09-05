<template>
<doter :foo='faza'></doter>
	<input type="text" ref="gott">

  <button @click='fox' class="opo" :class='{spg:foxy}'>Ok</button>

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

      ],
      foxy:false
    }
  },
  methods:{
    fox(){
     console.log(this.$refs.gott.value=555) 
      this.foxy=true
    }
  }
}
</script>

<style lang="css" scoped>
  .opo{
    color: red;
  }

.spg{
  color: gold;
}

</style>
