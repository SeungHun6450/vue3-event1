<template>

<!-- example 1 -->
<!-- $event 객체를 직접 명시 -->
  <!-- <button @click="handler('hi', $event)"> -->
    <!-- Click 1 -->
  <!-- </button> -->
  <!-- <button @click="handler('what', $event)"> -->
    <!-- Click 2 -->
  <!-- </button> -->

<!-- example 2 -->
  <button @click="handlerA(), handlerB()">
    Click me!
  </button>
</template>

<script>
// https://v3.ko.vuejs.org/guide/events.html#%E1%84%8B%E1%85%B5%E1%84%87%E1%85%A6%E1%86%AB%E1%84%90%E1%85%B3-%E1%84%8E%E1%85%A5%E1%86%BC%E1%84%8E%E1%85%B1

// example 1
// export default {
//   methods: {
//     handler(msg, event) {
//       console.log(msg)
//       console.log(event)
//     }
//   }
// }


// example2
export default {
  methods: {
    handlerA() {
      console.log('A')
    },
    handlerB() {
      console.log('B')
    }
  }
}
</script>