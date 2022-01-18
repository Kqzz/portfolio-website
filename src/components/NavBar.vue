<script>
export default {};
</script>

<template>
  <div class="navbar">
    <img src="../assets/logo.gif" alt="logo" class="logo" />
    <div class="nav-links">
      <a href="#projects">projects</a>
      <a href="#contact">contact</a>
    </div>
  </div>
</template>

<style scoped>
.logo {
  border-radius: 50%;
  float: left;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 110%;
  margin-right: 10%;
  margin-left: 10%;
}

.nav-links {
  display: flex;
}

a {
  margin: 1rem;
  color: #181618;
}
</style>
