<template>
  <div>
    <div class="menu">
    <div class="menu--content size margin container wrap align-items-center justify-content-between">
      <div>
        <h1> Games Components Admin </h1>
      </div>

      <div class="container wrap align-center">
        <router-link :to="{ name: 'Create' }">Create</router-link>
      </div>
    </div>
  </div>

  <div class="size margin content">
    <router-view/>
  </div>
  </div>
</template>
<script>
export default {
  name: "Main"
}
</script>
<style lang="scss" scoped>
a {
  color: #2c3e50;
  margin: 10px;
  text-decoration: none;
  &:hover {
    color: #42b983;
  }
}
.menu {
  border-bottom: 1px solid #ddd;
  margin-bottom: 50px;
}
.menu--content {
  min-height: 70px;
}
</style>
