<!--
 * @Description: 用户信息
 * @Author: suyh
 * @Date: 2021-06-22 14:38:59
 * @LastEditors: suyh
 * @LastEditTime: 2021-06-22 21:29:36
-->
<template>
  <div class="user_contain">
    <div class="container_left">
      <a-menu
        v-model:selectedKeys="selectedKeys"
        mode="inline"
        theme="light"
        style="width: 190px">
        <a-menu-item key="1">
          个人资料
        </a-menu-item>
        <a-menu-item key="2">
          账户设置
        </a-menu-item>
      </a-menu>
    </div>
    <div class="container_right">
      <!-- <route-view></route-view> -->
      <div >

      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  data() {
    return {
      selectedKeys: ["1"],
    };
  },
});
</script>

<style lang="scss" scoped>
.user_contain {
  width: 90%;
  margin: 24px auto;
  background-color: rgb(255, 255, 255);
  .container_left {
    width: 190px;
    height: 300px;
    float: left;
    border-right: 1px solid #f0f0f0;
  }
  .container_right {
    width: 100%;
    height: 300px;
    padding-left: 200px;
  }
}
</style>