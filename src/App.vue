<template>
  <UserCard msg="User Card" :usuario="usuario" :correo="correo" :biografia="biografia"/>
</template>

<script>
import UserCard from './components/UserCard.vue'

export default {
  name: 'App',
  components: {
    UserCard
  },
  data(){
    return{
      usuario:"Juan",
      correo:"juanmazon@correo.com",
      biografia:"They'll tell you now you're the lucky one"
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
