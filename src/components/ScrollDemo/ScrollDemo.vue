<template>
  <div class="ads-position">
    <ul>
      <li>Top 1</li>
      <li>Top 2</li>
      <li>Normal</li>
      <li>Bottom 1</li>
      <li>Bottom 2</li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: "ScrollDemo"
  }
</script>


<style lang="scss" scoped>
  .ads-position {
    overflow: auto;
    position: relative;
    width: 400px;
    height: 280px;
    outline: 1px solid #3c9;

    ul {
      padding: 200px 0;
      margin: 0
    }

    li {
      position: sticky;
      height: 40px;
      line-height: 40px;
      text-align: center;
      color: #fff;

      &:nth-child(1) {
        top: 0;
        z-index: 9;
        background-color: #f66;
      }

      &:nth-child(2) {
        top: 40px;
        z-index: 9;
        background-color: #66f;
      }

      &:nth-child(3) {
        background-color: #f90;
      }

      &:nth-child(4) {
        bottom: 0;
        z-index: 9;
        background-color: #09f;
      }

      &:nth-child(5) {
        bottom: 40px;
        z-index: 9;
        background-color: #3c9;
      }
    }
  }
</style>
