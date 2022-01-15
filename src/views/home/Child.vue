<template>
<div>
  <div>Child component</div>
  <p>my Name is {{myName}}</p>
  <input type="text" v-model="name">
  <button @click="$emit('changeName', name)">Change Name</button>
</div>
</template>

<script>
export default {
    props:['myName'],
    data(){
        return {
            name: ''
        }
    }
}
</script>

<style>

</style>