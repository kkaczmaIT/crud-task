<template>
    <div id="hero-header">
        <div style="margin: calc(10% + 5.6px)" class="container-hero-section d-flex column-direction justify-content-center align-items-center p-1">
          <header>
            <div class="hero-content">
                <h1 class="heading">{{ headerTitle }}</h1>
                <p class="text"> {{ headerText }}</p>
            </div>
          </header>
        </div> 
    </div>
</template>

<script>
    export default {
        name: 'TheHeroHeader',
        props: {
            headerTitle: {
                type: String,
                required: true
            },
            headerText: {
                type: String,
                required: false 
            }
        }
    }
</script>

<style lang="scss">
    @import '@/assets/scss/global';

    .container-hero-section {
      border: 6px solid $var-secondary;
      color: $var-dark;
      border-radius: 2px;
      width: 75%;
      header {
        width: 75%;
      }
    }
</style>