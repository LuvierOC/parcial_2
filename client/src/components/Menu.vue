<template>
  <div class="ui secondary menu">
    <div class="ui container">
      <div class="left menu">
        <router-link class="item" to="/">
          <img
            class="ui small image"
            src="../assets/logo.png"
            alt="Ecommerce"
          />
        </router-link>
      </div>
      <div class="rigth menu">
        <router-link class="item" to="/login"> Iniciar sesion </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Menu",
};
</script>

<style lang="scss" scoped>
.ui.menu.secondary {
  background-color: #5ae08e;
  .item {
    color: #fff;
    &:hover {
      color: #1fa1f1;
    }
  }
  .menu.left {
    width: 50%;

    .ui.image {
      width: 100px;
    }
  }
  .menu.right {
    width: 50%;
    justify-content: flex-end;
  }
}
</style>
