<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Selector de Usuario: Desarrolla un componente UserCard que acepte props para nombre de usuario, correo y biografía,
      y los muestre en un formato de tarjeta de perfil.
    </p>
    <h3>Installed CLI Plugins</h3>



  </div>
</template>

<script>
export default {
  name: 'UserForm',
  props: {
    msg: String,
    usuario: String,
    correo: String,
    biografia: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

</style>
