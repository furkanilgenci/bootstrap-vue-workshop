<script>
import CarCard from './components/CarCard.vue'

export default {
  name: 'App',
  data() {
    return {
      cars: [
        { name: 'audi a3', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
        { name: 'BMW i8', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
        { name: 'Ferrari', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
        { name: 'Mercedes E220', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
        { name: 'Masserati', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
        { name: 'Jaguar', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
        { name: 'Toyota', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
        { name: 'Honda', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco' },
      ]
    }
  },
  async created() {
    // const res = await ....
    // this.cars = res.data;
  },
  components: {
    CarCard
  }
}
</script>

<template lang="pug">
  #app
    h2.available-cars-title Available cars
    .container
      .row
        .col-12.col-lg-6.col-xl-4(v-for="car in cars")
          CarCard(:name="car.name" :description="car.description")
  </div>
</template>

<style>
#app {
  margin: 24px;
}

.available-cars-title {
  color: green;
  margin-bottom: 24px;
}
</style>
