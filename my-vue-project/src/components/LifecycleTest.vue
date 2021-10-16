<template>
  <h1>This is a Lifecycle test</h1>
</template>

<script>
  export default {
    name: 'LifecycleTest',
    props: ['numOfClicks'],
    beforeCreate() {
      console.log('In beforeCreate')
    },
    created() {
      console.log('In created')
    },
    beforeMount() {
      console.log('In beforeMount')
    },
    mounted() {
      console.log('In mounted')
    },
    beforeUpdate() {
      console.log('In beforeUpdate')
    },
    updated() {
      console.log('In updated')
    },
    beforeUnmount() {
      console.log('In beforeUnmount')
    },
    unmounted() {
      console.log('In unmounted')
    },
  }
</script>
