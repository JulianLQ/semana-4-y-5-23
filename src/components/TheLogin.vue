<template>
  <div>
    <form>

      <div class="form-group">
        <label for="exampleInputEmail1">Dirección electrónica</label>
        <input
          v-model="login.email"
          type="email"
          class="form-control"
          id="exampleInputEmail1"
          aria-describedby="emailHelp"
          placeholder="Ingresa tu e-mail"/>
        <small id="emailHelp" class="form-text text-muted"
          >Puedes estar tranquilo, no compartiremos tus datos.</small>
      </div>

      <div class="form-group">
        <label for="exampleInputPassword1">Contraseña</label>
        <input
          v-model="login.password"
          type="password"
          class="form-control"
          id="exampleInputPassword1"
          placeholder="Contraseña"/>
      </div>

      <!-- <pre>
        {{ login }}
      </pre> -->

      <!-- <div class="form-group form-check">
        <input type="checkbox" class="form-check-input" id="exampleCheck1" />
        <label class="form-check-label" for="exampleCheck1">Check me out</label>
      </div> -->

      <button type="submit" class="btn btn-primary">Ingresar</button>

    </form>
  </div>

</template>

<script>
  export default {
    name: "TheLogin",
    data(){
      return{
        login:{
          email: '',
          password: ''
        }
      }
    }
    
  };
</script>

<style scoped>

</style>
