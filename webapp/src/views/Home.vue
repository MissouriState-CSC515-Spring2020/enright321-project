<template>
  <div id="home">
    <div class="title">
      <h1>Recent Photo's</h1>
    </div>
    <Collection />
  </div>
</template>

<script>
import Collection from "@/components/Collection.vue";
export default {
  name: "home",
  components: {
    Collection
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 2;
  background: rgb(170, 170, 170);
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
}
h1 .title {
  padding: 0.5em;
  background: grey;
}
h1 #title {
  text-align: left;
  margin: 0em;
  background: grey;
}
</style>


