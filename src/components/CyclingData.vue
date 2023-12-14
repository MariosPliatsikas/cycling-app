<!-- src/components/CyclingData.vue -->

<template>
  <div>
    <!-- Add input fields for data points -->
    <label>Distance (km): <input v-model="distance" type="number" /></label>
    <label>Average Speed (km/h): <input v-model="averageSpeed" type="number" /></label>
    <label>Frequency (sessions/week): <input v-model="frequency" type="number" /></label>
    <label>Preferred Routes: <input v-model="preferredRoutes" type="text" /></label>

    <!-- Add a button to submit the data -->
    <button @click="submitData">Submit Data</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      distance: 0,
      averageSpeed: 0,
      frequency: 0,
      preferredRoutes: '',
    };
  },
  methods: {
    submitData() {
      // Implement logic to send data to the backend
      // You can use Axios or the fetch API to make API requests
      console.log('Data submitted:', {
        distance: this.distance,
        averageSpeed: this.averageSpeed,
        frequency: this.frequency,
        preferredRoutes: this.preferredRoutes,
      });
    },
  },
};
</script>

<style scoped>
/* Add styling if necessary */
</style>

