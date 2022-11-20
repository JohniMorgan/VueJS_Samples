<template>
  <div id="app">
    <MyComponent/>
  </div>
  
</template>

<script>
//import MyComponent from './components/MyComponent';
import ProductCounter from './components/ProductCounter';
export default {
  name: 'App',
  components: {
    ProductCounter
  }
}
</script>
