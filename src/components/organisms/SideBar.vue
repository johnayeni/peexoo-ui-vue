<template>
  <div class="sidebar">
    <img :src="logo" alt="Pexxo logo" class="sidebar__logo" width="200">
    <ul class="sidebar__links">
      <li v-for="(link, index) in links" :key="index" :class="link.active ? `sidebar__link active`: `sidebar__link`" v-on:click="toggleActiveLink(link.name)">
        <i :class="`ion-md-${link.icon}`"></i>
        <span>{{ link.name }}</span>
      </li>
    </ul>
    <p>&copy; Peexoo.ai</p>
  </div>  
</template>

<script>
import logo from '../../assets/img/logo.png';
import links from '../../data/links.json';
export default {
 data() {
   return {
     logo,
     links,
   }
 },
 methods: {
   toggleActiveLink(name) {
     this.links = this.links.map(link => {
       if(link.name === name) {
         return { ...link, active: true }
       }
         return { ...link, active: false }
     })
   }
 }
}
</script>
