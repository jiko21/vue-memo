<template>
  <div class="form">
    <input class="radius" type="text"/>
    <button class="radius">Add</button>
  </div>
</template>
<script>
export default {
  name: 'Form',
  props: [],
  data() {
    return {
    }
  },
  methods: {
  }
}
</script>
<style scoped>
.form {
  display: flex;
  height: 50px;

  justify-content: space-around;
  margin: 0 auto;
    display: flex;

}
input {
  font-size: 2.5em;
  width: 80%;
}
button {
  background-color: #21b9ff;
  color: #fff;
  font-size: 1.2em;
  font-weight: bold;
  width: 20%;
  padding: 0;
}
.radius {
  border-radius: 10px;
}
</style>
