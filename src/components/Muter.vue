<template>
<doter v-model='got'></doter>
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
      got:''
    }
  }
}
</script>

<style lang="css" scoped>
</style>
