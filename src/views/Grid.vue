<template>
  <div class="">
    <h1>Grid</h1>
    <div class="foo">
      <div class="bar">
        <div class="baz" v-for="i in 15" :key="i">{{ i }} item</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
.foo {
  @include grid-container;
  outline: 1px solid blue;
  .bar {
    @include grid-row;
    .baz {
      box-shadow: 0 0 35px -2px black;
      @include grid-item;
      @include col-desktop(2);
      @include col-tablet(6);
      @include col-mobile(12);
      @include media-phone {
        margin-top: 5px;
        margin-bottom: 5px;
      }
      @include media-tablet {
        margin-top: 10px;
        margin-bottom: 10px;
      }
      @include media-desktop {
        margin-top: 15px;
        margin-bottom: 15px;
      }
      background-color: #222;
      color: #999;
      padding: 20px;
      text-align: center;
    }
  }
}
</style>
