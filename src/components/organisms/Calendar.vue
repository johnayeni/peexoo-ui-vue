<template>
  <div class="calender">
    <div class="calendar__date">
      <p>
        <i class="ion-md-play margin-h-10 invert"></i>
        <i class="ion-md-play margin-h-10"></i>
        <span>September 2019</span>
        <span class="tag margin-h-10">Today</span>
      </p>
    </div>
    <calender-sheet />
  </div>  
</template>

<script>
import CalenderSheet from '../molecules/CalenderSheet.vue'
export default {
  components: {
    CalenderSheet,
  }
}
</script>
