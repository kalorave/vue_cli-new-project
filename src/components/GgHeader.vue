<template>
  <header>
    <router-link exact active-class="active" tag="a" to="/">Home</router-link>
    <router-link active-class="active" tag="a" to="/about">About</router-link>
    <router-link active-class="active" tag="a" to="/grid">Grid</router-link>
  </header>
</template>

<style lang="scss" scoped>
header {
  padding: 30px;
  background-color: #a9fff4;
}
a {
  margin: 10px;
  border: 1px solid skyblue;
  padding: 10px;
  background-color: #c4fff7;
  color: #222;
  text-decoration: none;
  border-radius: 5px;
  cursor: pointer;
  transition: all 0.2s linear;
  &:hover {
    border-color: blue;
  }
  &.active {
    background-color: #26295F;
    color: #fff;
  }
}

</style>
