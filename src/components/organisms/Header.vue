<template>
 <div class="header">
   <a href="#">Explore Photos</a>
   <a href="#">Find a photographer</a>
   <i class="ion-md-paper"></i>
   <i class="ion-ios-notifications-outline"></i>
   <i class="ion-ios-mail"></i>
   <img :src="avatar" alt="Bamidele Ali" class="avatar">
   <p>Bamidele</p>
   <i class="ion-ios-arrow-down"></i>
  </div>  
</template>

<script>
import avatar from '../../assets/img/avatar.png';
export default {
 data() {
   return {
     avatar,
   }
 }
}
</script>
