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
    <div class="calender__sheet">
      <div v-for="(day, index) in days" :key="index" class="calender__sheet-item">
        <p>{{ day }}</p>
      </div>
      <div class="calender__sheet-item">
        <p>1</p>
      </div>
      <div class="calender__sheet-item filled">
        <p>2</p>
        <p class="info">
          Mrs. Steven daugther's wedding photography
        </p>
      </div>
      <div v-for="(day, index) in Array.from(Array(25), (value, i) => i + 3)" :key="`${index}-unique`" class="calender__sheet-item">
        <p>{{ day }}</p>
      </div>
      <div class="calender__sheet-item filled">
        <p>28</p>
        <p class="info">
          Mrs. Steven daugther's wedding photography
        </p>
      </div>
      <div v-for="(day, index) in Array.from(Array(2), (value, i) => i + 29)" :key="`${index}-unique-1`" class="calender__sheet-item">
        <p>{{ day }}</p>
      </div>
      <div v-for="(day, index) in Array.from(Array(5), (value, i) => i + 30)" :key="`${index}-unique-2`" class="calender__sheet-item">
      </div>
    </div>
  </div>  
</template>

<script>
import days from '../../data/days.json';
export default {
  data() {
    return {
      days,
    }
  },
}
</script>
