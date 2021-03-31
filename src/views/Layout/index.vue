<!--
 * @Description: 上中下布局
 * @Author: suyh
 * @Date: 2021-03-31 11:32:35
 * @LastEditors: suyh
 * @LastEditTime: 2021-03-31 15:17:28
-->
<template>
  <a-layout id="baseLayout">
    <a-layout-header>
      <div class="logo">SBLOG</div>
      <a-menu
        mode="horizontal"
        :default-selected-keys="['1']"
        :style="{ lineHeight: '64px' }"
      >
        <a-menu-item key="1">
          <router-link to="/">发现</router-link>
        </a-menu-item>
        <a-menu-item key="2">
          <router-link to="/collection">收藏</router-link>
        </a-menu-item>
        <a-menu-item key="3">
          <router-link to="/message">消息</router-link>
        </a-menu-item>
      </a-menu>
    </a-layout-header>
    <a-layout-content :style="{ padding: '0 50px', marginTop: '64px' }">
      <router-view/>
    </a-layout-content>
    <a-layout-footer :style="{ textAlign: 'center' }">
      Ant Design ©2018 Created by Ant UED
    </a-layout-footer>
  </a-layout>
</template>
<style lang="scss" scoped>
#baseLayout{
  background-color: #fff;
  .ant-layout-header{
    position: absolute;
    z-index: 1;
    width: 100%;
    height: 66px;
    background-color: #fff;
    border-bottom: 1px solid #f0f0f0;
  }
  .logo{
    width: 120px;
    height: 31px;
    color: #1890ff;
    line-height: 31px;
    text-align: center;
    font-size: 24px;
    font-weight: 700;
    background: #fff;
    margin: 16px 24px 16px 0;
    float: left;
  }
  
}
</style>