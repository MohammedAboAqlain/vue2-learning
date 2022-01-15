<template>
  <div class="home">
    <p>Home Page</p>
    <Child myName="Mohammed" @changeName="changeName" />
  </div>
</template>

<script>
// @ is an alias to /src
import Child from './Child.vue';

export default {
  name: 'Home',
  components: {
    Child,
  },
  methods: {
    changeName(val) {
      console.log(val);
    },
  },
};
</script>
