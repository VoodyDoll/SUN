<template>
  <button @click="go">OK</button>

  <p>{{goo}}</p>
  <p>Root-{{ item }}</p>
  <p>Father-{{dooda}} {{hoth}}</p>
  <!-- <p>{{go[0]}} {{go[1]}}</p> -->
  <p>{{aza}}</p>
  <sun></sun>
<!-- <div v-for='toy in toys'>
  <p ></p>
</div> -->
<!-- <doter :foo='faza' :ptah='boop'></doter> -->
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
      aza:[
      {valuess:'focuss',name:'Фикус',age:10},
      {valuess:'loid',name:'Пальма',age:12},
      {valuess:'chankala',name:'Хвощ',age:13},
      {valuess:'zizan',name:'Пудра',age:14}

      ],
      foxy:false,
      gudariann:'',
      cill:'',
      boop:'',
      toys:[],
      dooda:'GOD',
      hoth:'GIISRA'
    }
  },
  methods:{
    fox(){
     this.$refs.gott.value=555
      this.foxy=true
    },
    human(){    

     this.boop=this.cill
    },
    // goo(){
    //   this.aza.push({valuess:'tyhg',name:'Ghg',age:100})
    // }
  },
  computed:{    
    goo(){     
      return this.aza.reduce((item,nin)=>(item=item+nin.age),0)
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
