<template>
  <!-- <input type="text" v-model='gudariann'> -->
  <!-- <input type="text" v-model="gudariann" name=""> -->
  <!-- <button @click='human'>Ok</button> -->
  <sun></sun>
<div v-for='toy in toys'>
  <p ></p>
</div>
<doter :foo='faza' :ptah='boop'></doter>
	<!-- <input type="text" ref="gott"> -->

  <!-- <button @click='fox' class="opo" :class='{spg:foxy}'>Ok</button> -->

</template>

<script>
import Doter from '@/components/Doter.vue'
import Sun from '@/components/Sun.vue'

export default {
components:{
   Doter,
   Sun
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
      foxy:false,
      gudariann:'',
      cill:'',
      boop:'',
      toys:[]
    }
  },
  methods:{
    fox(){
     this.$refs.gott.value=555
      this.foxy=true
    },
    human(){    

     this.boop=this.cill
    }
  },
  computed:{    
    gudariann(loo){
      console.log(loo)
     return this.boop=this.loo
    }
  }

// watch: {
//   cill(val){
//     this.boop=val
//   }
// }
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
