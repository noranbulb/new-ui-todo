<template>
  <div class="app">
    <div class="container">
      <div class="content">
        <h1 class="title">
          Neumorphism UI <br>
          Todo List!

          dev test 1
        </h1>
        <div class="input-area">
          <div class="input">
            <input type="text" />
          </div>
          <button>추가</button>
        </div>
        <div class="list">
          <div class="card" v-for="item in [1, 2, 3, 4]" :key="item">
            <h2>
              <span class="number">{{ item }}</span>
              <span class="date">2020.01.20</span>
            </h2>
            <p class="txt">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Enim beatae nihil consequuntur necessitatibus quaerat cupiditate fuga! Laboriosam, nulla deserunt in est doloribus officia, fugiat veritatis obcaecati rem reiciendis possimus fugit.
            </p>
            <div class="remote">
              <button>삭제</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {};
</script>

<style lang="scss" scoped>
// 71b9c1
// f6f5f1

  // --mainBlue: #4265ed;
  // --sky: #86adfc;
  // --bgColor: #f6f9fc;
  // --bgBtn: #f9fcfe;
  // --red:#fa5d5d;
  // --orange: #f27200;
  // --mint: #28c3d7;
  // --green: #02bc77;
.app {
  height: 100%;
  background: #71b9c1;
  padding: 10px;
  .container {
    height: 100%;
    border-radius: 20px;
    background: #71b9c1;
    box-shadow: inset 5px 5px 10px #609da4, inset -5px -5px 10px #82d5de;
    overflow: hidden;
    .content {
      height: 100%;
      padding: 0 25px;
      overflow: auto;
      -webkit-overflow-scrolling: touched;
      .title {
        margin-top: 80px;
        color: #f6f5f1;
      }
      .input-area {
        margin-top: 30px;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        .input {
          border-radius: 25px;
          background: #71b9c1;
          box-shadow: inset 5px 5px 10px #609da4, inset -5px -5px 10px #82d5de;
          height: 50px;
          padding: 0 25px;
          flex: 1;
          input {
            height: 100%;
            color: #f6f5f1;
            font-size: 18px;
            width: 100%;
          }
        }
        button {
          margin-left: 20px;
          border-radius: 10px;
          background: linear-gradient(145deg, #02c97f, #02a96b);
          box-shadow: 5px 5px 10px #609da4, -5px -5px 10px #82d5de;
          height: 40px;
          width: 50px;
          font-size: 18px;
          color: #f6f5f1;
          transition: all 0.3s;
          &:active {
            background: linear-gradient(145deg, #02a96b, #02c97f);
            box-shadow: 5px 5px 10px #609da4, -5px -5px 10px #82d5de;
          }
        }
      }
      .list {
        margin-top: 50px;
        .card {
          color: #f6f5f1;
          border-radius: 20px;
          background: #71b9c1;
          box-shadow: 5px 5px 10px #609da4, -5px -5px 10px #82d5de;
          padding: 20px;
          margin-bottom: 30px;
          h2 {
            border-bottom: 1px solid #f6f5f1;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            line-height: 28px;
            .number {
              flex: 1;
              font-size: 24px;
            }
            .date {
              float: right;
              font-size: 12px;
              opacity: 0.8;
            }
          }
          .txt {
            margin: 10px 0;
            font-size: 18px;
            padding: 0 5px;
            word-break: keep-all;
          }
          .remote {
            border-top: 1px solid #f6f5f1;
            padding-top: 20px;
            display: flex;
            button {
              margin-left: auto;
              color: #f6f5f1;
              height: 30px;
              width: 50px;
              font-size: 16px;
              border-radius: 10px;
              background: linear-gradient(145deg, #ff6464, #e15454);
              box-shadow: 5px 5px 10px #609da4, -5px -5px 10px #82d5de;
            }
          }
        }
      }
    }
  }
}
</style>
