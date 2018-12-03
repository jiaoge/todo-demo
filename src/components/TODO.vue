<template>
  <div style="height:100%;">
    <Todo-Head></Todo-Head>
    <div class="columns" style="height:calc(100% - 48px);">
      <div class="column is-narrow has-background-light" style="width: 290px;">
        <div
          class="level"
          style="margin-top:24px;margin-bottom:0px;padding-left:8px;"
        >
          <div class="level-left">
            <span class="icon has-text-link">
              <ion-icon name="menu" size="large"></ion-icon>
            </span>
          </div>
        </div>
        <div class="todo-group">
          <div class="level">
            <div class="level-left">
              <span class="icon"> <ion-icon name="sunny"></ion-icon> </span>
              <span>我的一天</span>
            </div>
            <div class="level-right"><span></span></div>
          </div>
          <div class="level">
            <div class="level-left">
              <span class="icon">
                <ion-icon name="star-outline"></ion-icon>
              </span>
              <span>重要</span>
            </div>
            <div class="level-right"><span></span></div>
          </div>
          <div class="level">
            <div class="level-left">
              <span class="icon"> <ion-icon name="calendar"></ion-icon> </span>
              <span>已计划日程</span>
            </div>
            <div class="level-right"><span>1</span></div>
          </div>
          <div class="level has-text-link	">
            <div class="level-left">
              <span class="icon"> <ion-icon name="home"></ion-icon> </span>
              <span>任务</span>
            </div>
            <div class="level-right"><span>4</span></div>
          </div>
        </div>

        <div class="todo-group">
          <div class="level">
            <div class="level-left">
              <span class="icon has-text-link">
                <ion-icon name="list-box"></ion-icon>
              </span>
              <span>Java Web</span>
            </div>
            <div class="level-right"><span></span></div>
          </div>
          <div class="level">
            <div class="level-left has-text-link">
              <span class="icon "> <ion-icon name="add"></ion-icon> </span>
              <input
                class="input is-small"
                type="text"
                placeholder="新建清单"
              />
            </div>
          </div>
        </div>

        <div class="level" style="bottom:0px;position: absolute;">
          <div class="level-left"><span>获取应用。</span></div>
        </div>
      </div>
      <!-- 任务列表 -->
      <div class="column" style="margin:12px;">
        <div class="level todo-list-top">
          <div class="level-left">
            <span
              class="has-text-link"
              style="font-size:20px;margin-right:12px;"
              >任务</span
            >
            <a href="#">...</a>
          </div>
          <div class="level-right" style="padding-right:12px;">
            <span class="icon has-text-link">
              <ion-icon name="funnel"></ion-icon>
            </span>
            <a href="#"> 排序 </a>
          </div>
        </div>

        <div class="todo-list">
          <div class="level">
            <div class="level-left">
              <span class="icon">
                <ion-icon name="radio-button-off"></ion-icon>
              </span>
              <div class="level-item" style="margin-left:12px;">
                <div>
                  <p>测试工程</p>
                  <p class="heading">2018.12.29</p>
                </div>
              </div>
            </div>
            <div class="level-right">
              <span class="icon">
                <ion-icon name="star-outline"></ion-icon>
              </span>
            </div>
          </div>
          <div class="tabs"><ul></ul></div>
          <div class="level">
            <div class="level-left">
              <span class="icon">
                <ion-icon name="checkmark-circle-outline"></ion-icon>
              </span>
              <div class="level-item" style="margin-left:12px;">
                <div>
                  <p>测试工程</p>
                  <p class="heading">2018.12.29</p>
                </div>
              </div>
            </div>
            <div class="level-right">
              <span class="icon">
                <ion-icon name="star-outline"></ion-icon>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TodoHead from "TodoHead";
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  },
  component: {
    TodoHead: TodoHead
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.todo-nav {
  background: #346fef;
  color: #ffffff;
  height: 48px;
}
.level {
  margin: 0;
  padding: 0;
}
.columns {
  margin: 0;
  padding: 0;
}

.columns:not(:last-child) {
  margin: 0;
}
.column {
  margin: 0;
}
.todo-group {
  margin-top: 24px;
  font-size: 14px;
}

.todo-group .level {
  margin-bottom: 12px;
}
.todo-group .level .icon {
  margin-right: 8px;
}
ion-icon {
  font-size: 21px;
}

.todo-list-top {
  font-size: 14px;
}

.todo-list .level {
  margin: 4px;
  font-size: 14px;
}

.todo-list .tabs {
  margin: 0px;
}
</style>
