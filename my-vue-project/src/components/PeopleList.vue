<template>
  <div>
    <h1>People List</h1>
    <PeopleListItem />
    <PeopleListItem />
    <PeopleListItem />
  </div>
</template>

<script>
  import PeopleListItem from './PeopleListItem.vue'

  export default {
    name: 'PeopleList',
    components: {
      PeopleListItem,
    },
  }
</script>
