<template>
  <div id="app">
    <!-- <div class="navbar navbar-primary">
      <div class="navbar-logo"><a href="#">Logo</a></div>
      <nav class="nav-menu">
        <ul class="nav-list">
          <li class="nav-item active"><a href="#" class="nav-link">Link 1</a>
          <span class="d-block decorated-line-link"></span>
          </li>
          <li class="nav-item"><a href="#" class="nav-link">Link 2</a>
            <span class="d-block decorated-line-link"></span>
          </li>
          <li class="nav-item"><a href="#" class="nav-link">Link 3</a>
            <span class="d-block decorated-line-link"></span>
          </li>
          <li class="nav-item"><a href="#" class="nav-link">Link 4</a>
            <span class="d-block decorated-line-link"></span>
          </li>
        </ul>

  
      </nav>

      <div class="toggler">
          <div class="toggler-icon">
            <span class="bar"></span>
            <span class="bar"></span>
            <span class="bar"></span>
          </div>
        </div>
    </div> -->
    <NavBar></NavBar>
    <div class="row" :style="{backgroundImage: 'url(' + imgHome + ')', backgroundSize: 'cover', backgroundRepeat: 'no-repeat', backgroundPosition: 'center'}" style="min-height: 400px">
      <div class="col-sm-10 col-md-4 col-lg-5 col-xl-5 d-flex column-direction justify-content-center align-items-center">
        <div class="container-hero-section d-flex column-direction justify-content-center align-items-center p-1">
          <header>
            <div class="hero-content">
                <h1 class="heading">Add offer of Your company</h1>
                <p class="text">Offer Your company delivered to Your clients in comfortable way. Fast & Easily & Effective.</p>
            </div>
          </header>
        </div>    
      </div>
      <div class="col-sm-10 col-md-6 col-lg-5 col-xl-5">
        <TheForm></TheForm>
      </div>

      <div class="overlay"></div>
    </div>
        
  </div>
</template>

<script>
  import NavBar from './components/NavBar'
  import TheForm from './components/TheForm'
  export default {
    components: {
      NavBar,
      TheForm
    },
    data() {
      return {
        imgHome: require('@/assets/img/home.jpg')
      }
    },
    methods: {

    }
  }
</script>

<style scoped lang="scss">
  @import './assets/scss/global';

  .row {
    position: relative;
    z-index: 1;
    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      min-height: 100%;
      background-color: $var-additional;
      opacity: .5;
      z-index: 2;
    }

    @for $n from 1 through 10 {
        .col-#{$n}, .col-sm-#{$n}, .col-md-#{$n}, .col-lg-#{$n}, .col-xl-#{$n}  {
            z-index: 3;
        }
    }

    .container-hero-section {
      border: 6px solid $var-secondary;
      color: $var-dark;
      border-radius: 2px;
      width: 75%;
      header {
        width: 75%;
      }
    }
    
  } 

</style>
