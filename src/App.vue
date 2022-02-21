<template>
  <div id="app">

    <HeaderComponent/>
    <ContentComponent/>
    <ShopComponent/>
    <FooterComponent class="footer"/>

  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import ContentComponent from './components/ContentComponent.vue'
import ShopComponent from './components/ShopComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    ContentComponent,
    ShopComponent,
    FooterComponent
  }
}
</script>

<style lang="scss">
  @import "./assets/style/general.scss";


</style>
