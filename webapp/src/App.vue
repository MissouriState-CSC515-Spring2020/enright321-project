<template>
  <div id="app">
    <Header />
    <router-view />
    <div id="imgs"></div>
  </div>
</template>

<script>
import Header from "./components/layout/Header";

export default {
  name: "app",
  components: {
    Header
  },
  data() {
    return {};
  }
};
</script>


<style>
html {
  font-size: 20px;
}
body {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
a {
  color: #0094ff;
  text-decoration: none;
}
a:hover {
  color: #0074c6;
}

/*app is global styling*/
/* #app {
  color: black;
}

#imgs {
  width: "50%";
  display: block;
  margin-left: auto;
  margin-right: auto;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
.btn {
  display: inline-block;
  border: none;
  background: #555;
  color: #fff;
  padding: 7px 20px;
  cursor: pointer;
}
.btn:hover {
  background: #666;
} */
</style>
