<template>
<BasicLayouts>
   <div class="login">
        <h2>Iniciar sesion</h2>
        <form class="ui form">
           <div class="field"> 
             <input type="text"
              placeholder="nombre del usuario"/>
            </div> 
            <div class="field">
              <input type="password" placeholder="Contaseña"/>       
            </div>
            <button type="submit"
             class="ui button fluid primary"
             >Entrar
            </button>
        </form>   
        <router-link to="/register">crear una cuenta</router-link> 
  </div>
</Basiclayouts>
</template>

<script>
import BasicLayouts from '../layouts/BasicLayouts.vue';

export default {
    name:"login",
  components: { 
      BasicLayouts, 
   },   
};
</script>
<style lang= "scss" scode>
.login{
     text-align: center;
   >h2 {
      margin: 50px 0 30px 0;
  }
  .ui.form{
   max-width: 300px !important;
   margin: 0 auto;
   margin-bottom: 10px;
   input.error { 
    border-color: #faa;
    background-color: #ffeded;
   }
  }
}
</style>