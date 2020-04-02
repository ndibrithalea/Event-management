<template>
   <nav class="navbar navbar-expand-lg navbar-light">
    <a class="navbar-brand" href="">Event Management</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="nav navbar-nav ml-auto">
            <router-link to="/" class="nav-link">Home</router-link>
            <router-link to="/about" class="nav-link">About</router-link>

            <a href="" class="btn btn-dark text-white">Sign In</a>
        </ul>
    </div>
   </nav>
</template>
<script>
export default {
    name: 'Nav'
}
</script>
<style lang="scss" scoped>
  nav {
   
    a {
      font-weight: bold;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #d88d00;
      }
    }
  }
</style>