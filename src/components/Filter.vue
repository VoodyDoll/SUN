<template>
	<div class="container">
    <div class="row">
      <div class="col-md">
       <my-select v-model='selectedS' :options='sortOptions'></my-select>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {

  name: 'Filter',

  data () {
    return {
      selectedSort:'',
      sortOptions:[
        {value:'age',name:'От дешовых к дорогим'},
        {value:'age',name:'От дорогих к дешовым'}
      ],

    }
  },
  methods:{

  },
  computed:{
    selectedS(neww){
      this.$emit('revers',neww.value)
     console.log(neww)
     
    }
  }
}
</script>

<style lang="css" scoped>
</style>