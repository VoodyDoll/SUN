<template>
	 <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Наборы</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Роллы</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Горячие роллы</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Маки роллы</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Гунканы роллы</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Пиццы</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Wok</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Супы</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Салаты</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Закуски</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li>
        <li class="nav-item" v-if='case'>
          <button type="button" class="btn btn-outline-danger">КОРЗИНА</button>
        </li>
      </ul>
      <form class="d-flex" >
        <!-- поле поиска -->
        <input v-model='searchvalue' class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <!-- <button @click='searchr'  class="btn btn-outline-success" >Search</button> -->
      </form>
    </div>
  </div>
</nav>
</template>

<script>
export default {

  name: 'NavBar',

  data () {
    return {
      searchvalue:''
    }
  },
  methods:{
    // searchr(event){
    //   event.preventDefault()
    //   this.$emit('setcher',this.searchvalue)
    //   // console.log(this.searchvalue)
    //   this.searchvalue=''
    // }
  },
  watch:{
    searchvalue(){
      this.$emit('setcher',this.searchvalue)
    }
  }
}
</script>

<style lang="css" scoped>
</style>