<template>
  <view>
    <headbar left="more" :url="url" basic="最近打开"></headbar>
    <view class="main">
      <view class="dealList" v-for="(item, index) in dealList" :key="index">
        <dealItem :itemInfo="item"></dealItem>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      url: "/pages/work/menu/menu",
      dealList: [
        {
          title: "这是一张审批单",
          sub: "资金审批，望通过",
          type: "单位审批",
        },
        {
          title: "“张三”想加入单位",
          sub: "你好，我是市场部新员工张三",
          type: "好友申请",
        },
        {
          title: "“张三”想加入单位",
          sub: "你好，我是市场部新员工张三",
          type: "好友申请",
        },
        {
          title: "“张三”想加入单位",
          sub: "你好，我是市场部新员工张三",
          type: "好友申请",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
.main {
  margin-top: 20upx;
  display: flex;
  flex-direction: column;
  align-items: center;
  .dealList {
    margin-top: 20upx;
  }
}
</style>
