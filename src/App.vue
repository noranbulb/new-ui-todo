<template>
  <div class="app">
    <div class="container">
      <div class="input-area">
        input
      </div>
      <div class="content">
        <div class="card" v-for="item in [1, 2, 3, 4, 5, 6]" :key="item">
          <h1>{{ item }}</h1>
          <p>card</p>
          <p>card</p>
          <p>card</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {};
</script>

<style lang="scss" scoped>
.app {
  height: 100%;
  background-color: #71b9c1;
  .container {
    height: 100%;
    background-color: #f6f5f1;
    --padding: 10px;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    .input-area {
      background-color: #f6f5f1;
      box-shadow: inset 5px 5px 10px #d1d0cd, inset -5px -5px 10px #ffffff;
      height: 50px;
      border-radius: 10px;
      margin-bottom: 15px;
      padding: 10px;
      margin: 15px;
    }
    .content {
      flex: 1;
      border-radius: 10px;
      background-color: #f6f5f1;
      overflow: auto;
      padding: 0 15px;
      .card {
        border-radius: 20px;
        background: #f6f5f1;
        box-shadow: 5px 5px 10px #d1d0cd, -5px -5px 10px #ffffff;
        padding: 10px;
        margin-bottom: 30px;
      }
    }
  }
}
</style>
