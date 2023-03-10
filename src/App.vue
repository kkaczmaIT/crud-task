<template>
  <div id="app">
    
    <NavBar></NavBar>
    <div class="row" :style="{backgroundImage: 'url(' + imgHome + ')', backgroundSize: 'cover', backgroundRepeat: 'no-repeat', backgroundPosition: 'center'}" style="min-height: 400px">
      <div class="col-sm-10 col-md-4 col-lg-5 col-xl-5 d-flex column-direction justify-content-start align-items-center">
        <TheHeroHeader headerTitle="Add offer of Your company" headerText="Offer Your company delivered to Your clients in comfortable way. Fast & Easily & Effective."></TheHeroHeader>
      </div>
      <div class="col-sm-10 col-md-6 col-lg-5 col-xl-5">
        <TheForm></TheForm>
      </div>

      <div class="overlay"></div>
    </div>
    <footer class="footer-primary p-1">
      Application create as a project to portfolio
    </footer>
  </div>
</template>

<script>
  import NavBar from './components/NavBar'
  import TheForm from './components/TheForm'
  import TheHeroHeader from './components/TheHeroHeader'

  export default {
    components: {
      NavBar,
      TheForm,
      TheHeroHeader
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
    
  } 

</style>
