<template>
  <div>
    <p>You have clicked the button {{ numberOfClicks }} times</p>
    <button @click="$emit('increment')">Click me!</button>
  </div>
</template>

<script>
  export default {
    name: 'CounterButton',
    props: ['numberOfClicks'],
  }
</script>
