<template>
  <div class="app">
    <side-bar/>
    <div class="content">
      <Header />
      <availability />  
    </div>    
  </div>
</template>

<script>
import SideBar from "./components/organisms/SideBar.vue";
import Header from "./components/organisms/Header.vue";
import Availability from './components/templates/Availability.vue';
export default {
  name: 'app',
  components: {
    SideBar,
    Header,
    Availability,
  }
}
</script>