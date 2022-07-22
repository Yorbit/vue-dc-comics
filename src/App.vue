<template>
  <section id="app">
    <BaseHeader/>
    <BaseMain/>
    <BaseFooter/>
  </section>
</template>

<script>

import BaseHeader from './components/BaseHeader.vue'
import BaseMain from './components/BaseMain.vue'
import BaseFooter from './components/BaseFooter.vue'


export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooter,
  }
}
</script>

<style lang="scss">
  @import'./styles/general.scss';
  @import'./styles/colors.scss';


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
};
</style>
