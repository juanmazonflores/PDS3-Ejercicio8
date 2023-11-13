<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Selector de Usuario: Desarrolla un componente UserCard que acepte props para nombre de usuario, correo y biografía,
      y los muestre en un formato de tarjeta de perfil.
    </p>
    <h3>Informacion</h3>
    <div class="card">
      <img src="../assets/img_avatar.png" alt="Avatar" style="width:100%">
      <div class="container">
        <h4><b>Usuario</b></h4>
        <p>{{usuario}}</p>
        <h4><b>Correo</b></h4>
        <p>{{correo}}</p>
        <h4><b>Biografia</b></h4>
        <p>{{biografia}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'UserCard',
  props: {
    msg: String,
    usuario: {
                type: String
            },
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
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 20%;
  margin: 0 auto;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.container {
  padding: 2px 16px;
}

</style>
