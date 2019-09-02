<template>
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
    <div v-for="(day, index) in Array.from(Array(8), (value, i) => i + 3)" :key="`${index}-unique`" class="calender__sheet-item">
      <p>{{ day }}</p>
    </div>
    <div class="calender__sheet-item filled wide">
      <div class="space-between" style="width: 100%">
        <p>11</p>
        <p>12</p>
        <p>13</p>
      </div>
      <p class="info">
        Mrs. Steven daugther's wedding photography
      </p>
    </div>
    <div v-for="(day, index) in Array.from(Array(14), (value, i) => i + 14)" :key="`${index}-unique-1`" class="calender__sheet-item">
      <p>{{ day }}</p>
    </div>
    <div class="calender__sheet-item filled">
      <p>28</p>
      <p class="info">
        Mrs. Steven daugther's wedding photography
      </p>
    </div>
    <div v-for="(day, index) in Array.from(Array(2), (value, i) => i + 29)" :key="`${index}-unique-2`" class="calender__sheet-item">
      <p>{{ day }}</p>
    </div>
    <div v-for="(day, index) in Array.from(Array(5), (value, i) => i + 30)" :key="`${index}-unique-3`" class="calender__sheet-item">
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
