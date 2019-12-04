<template>
  <div class="home">
    <header>消息</header>
    <input type="text" placeholder="请输入关键字">
    <div class="main" v-for="item in list" :key="item">
      <img :src="item.img" alt />
      <span>{{item.title}}</span>
      <span>{{item.des}}</span>
      <p>{{item.time}}</p>
    </div>
    <div class="footer">
      <router-link to="/" tag="span">首页</router-link>
      <router-link to="/about" tag="span">分类</router-link>
      <router-link to="/my" tag="span">我的</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      list: [
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        },
        {
          img: "https://f11.baidu.com/it/u=1243293019,1807664460&fm=72",
          title: "我的同桌",
          des: "作业写完了没 6666",
          time: "17:00"
        }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.home {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
}
header {
  width: 100%;
  height: 50px;
  background: skyblue;
  text-align: center;
  line-height: 50px;
  font-size: 30px;
}
.main {
  flex: 1;
  img{
    width: 200px;
    height: 200px;
  }
}
.footer {
  width: 100%;
  height: 60px;
  background: hotpink;
  text-align: center;
  line-height: 60px;
  span {
    padding: 50px;
  }
}
</style>