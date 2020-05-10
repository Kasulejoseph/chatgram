<template>
<div class="container">
  <section class="navbar hello sticky-top nav-pills nav-fill">
      <h2 class="nav-item">Instagram</h2>
      <div class="form-group nav-item">
        <input type="search" class="form-control" name="Search" id="" placeholder="search">
      </div>
      <section class="nav-item">
        <i class="fas fa-home fa-2x mr-4"></i>
        <i class="fas fa-camera fa-2x mr-4"></i>
        <i class="far fa-heart fa-2x mr-4"></i>
        <i class="far fa-user-circle fa-2x"></i>
      </section>
  </section>
</div>
</template>

<script>
export default {
  name: 'NavNar',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
