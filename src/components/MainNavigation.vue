<template>
  <div class="nav-container">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style scoped>
.nav-container {
  display: flex;
  justify-content: center;
}

#nav {
  display: flex;
  align-items: center;
  justify-content: space-around;
  max-width: 40rem;
  min-width: 20rem;
}

a {
  font-size: 2rem;
  margin-bottom: 0.5rem;
  text-decoration: none;
  border-bottom: 1px solid #00baff;
}
</style>
