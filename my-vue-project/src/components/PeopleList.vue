<template>
  <div>
    <h1>People List</h1>
    <PeopleListItem :person="person1" />
    <PeopleListItem :person="person2" />
    <PeopleListItem :person="person3" />
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
        person1: { name: 'Edward', age: 100, hairColor: 'black' },
        person2: { name: 'John', age: 50, hairColor: 'green' },
        person3: { name: 'Nancy', age: 34, hairColor: 'red' },
      }
    },
  }
</script>
