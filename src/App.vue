<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <NevBar />
  <FooterSection />
  <DireCtive />
  <LoOp />
  <div id="app">
    <ToggleText />
  </div>
  <AniMate />
</template>

<script>
import AniMate from './components/AniMate'
import ToggleText from './components/ToggleText.vue'
import HelloWorld from './components/HelloWorld.vue'
import NevBar from './components/NevBar'
import FooterSection from './components/FooterSection'
import DireCtive from './components/DireCtive'
import LoOp from './components/LoOp'
export default {
  name: 'App',
  components: {
    HelloWorld,
    NevBar,
    FooterSection,
    DireCtive,
    LoOp,
    ToggleText,
    AniMate
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
