<template>
  <div>
    <h1>Employee of the Month</h1>
    <div v-if="personData">
      <h3>{{ personData.name.first }} {{ personData.name.last }}</h3>
    </div>
  </div>
</template>

<script>
  import axios from 'axios'

  export default {
    name: 'EmployeeOfTheMonthPage',
    data() {
      return {
        personData: null,
      }
    },
    created() {
      axios
        .get('https://randomuser.me/api/')
        .then(response => (this.personData = response.data.results[0]))
    },
  }
</script>
