<template>
  <div class="list">
    <!-- ここがリストのタイルになります-->
    <div class="todo-card">
    </div>
  </div>
</template>
<script>
export default {
  name: 'List',
  props: [],
}
</script>
<style scoped>
.todo-card {
  border-radius: 10px;
  box-shadow: 0 4px 10px 4px rgba(0,0,0,0.1);
  min-height: 100px;
  position: relative;
  margin: 0 auto;
}
h2 {
  font-size: 2.2em;
  vertical-align: middle;
}
button.danger {
  background-color:#ff3b58;
  border-radius: 0 0 10px 10px;
  bottom: 0;
  color: white;
  font-size: 1.5em;
  font-weight: bold;
  height: 40px;
  position: absolute;
  right: 0;
  width: 100%;
}
</style>
