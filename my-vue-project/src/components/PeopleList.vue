<template>
  <div>
    <h1>People List</h1>
    <PeopleListItem
      v-for="person in people"
      :key="person.name"
      :person="person"
    />
  </div>
</template>

<script>
  import PeopleListItem from './PeopleListItem.vue'

  export default {
    name: 'PeopleList',
    components: {
      PeopleListItem,
    },
    data() {
      return {
        people: [
          { name: 'Edward', age: 100, hairColor: 'black' },
          { name: 'John', age: 50, hairColor: 'green' },
          { name: 'Nancy', age: 34, hairColor: 'red' },
        ],
      }
    },
  }
</script>

<style scoped>
  h1 {
    color: red;
  }
</style>
