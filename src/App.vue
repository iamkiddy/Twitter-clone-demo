<template>
  <div class="app">
    <Menu/>
  </div>
</template>

<script>
import Menu from "./components/Menu.vue"

export default {
  name: 'App',
  components: {
    Menu
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

*{
  margin:0px;
  padding:0px;
  box-sizing:border-box;
  font-family: "Roboto" ,sans-serif;
}
.app{
  display:grid;
  grid-template-columns: repeat(3 ,1fr);
  margin-top:15px;
}

</style>
