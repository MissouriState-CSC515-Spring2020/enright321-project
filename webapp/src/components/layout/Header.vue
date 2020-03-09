<template>
  <header class="header">
    <h1>Photography Collection</h1>
    <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/category">Categories</router-link>|
      <router-link to="/detail">Details</router-link>
    </div>
  </header>
</template>

<script>
export default {
  default() {
    return {
      name: "Header"
    };
  }
};
</script>

<style scoped>
.header {
  background: rgb(0, 34, 13);
  color: #fff;
  text-align: center;
  padding: 10px;
}
.header a {
  color: #fff;
  padding-right: 5px;
  text-decoration: none;
}
.header h1 {
  color: rgb(255);
}
</style>