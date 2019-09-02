<template>
  <div class="container">
    <h2>Availability</h2>
    <div class="space-between">
      <view-changer/>
      <div class="flex-row">
        <input type="search" class="input grow" placeholder="search">
        <button class="btn margin-h-10">
          <i class="ion-md-add"></i>
          Add Schedule</button>
      </div>
    </div>
    <calendar/>
  </div>
</template>

<script>
import ViewChanger from '../molecules/ViewChanger.vue';
import Calendar from '../organisms/Calendar.vue';

export default {
 components: {
   ViewChanger,
   Calendar,
 }
}
</script>
