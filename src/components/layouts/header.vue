
<template>
  <header class="header">
    <h2>{{title}}</h2>
  </header>
</template>
<script>
export default {
  name: "header",
  data(){
      return {title:'test'}
  }
};
</script>
<style scoped>
/* Style the header */
.header {
  background-color: #666;
  padding: 30px;
  text-align: center;
  font-size: 35px;
  color: white;
}
</style>
