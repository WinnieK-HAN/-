# 微信小程序
WeChat miniprogram  demo

## 项目说明 ##
> 一个外卖订餐等周边服务的微信小程序
> 与饿了吗功能雷同

### ui框架
> 基于 官方拓展UI框架  WeUI组件库

### API 
> https://developers.weixin.qq.com/miniprogram/dev/framework/

### 项目特色
1.  地理定位（qqmapsdk = new QQMapWX）
2.  基地选择（组件picker 选择器）
3.  分页展示-触底加载（..addList）
4.  店铺菜谱展示（组件 vtabs）
5.  商品添加（减、清空）购物车-计算价格 （逻辑运算）
6.  评价打分 （根据分值计算星级 逻辑运算）
7.  **二维码生成 （订单二维码取餐）   二维码高亮**
8.  订单（组件 tabs）
9.  调查问卷 （表单 增删改查）
10. 质量检查 （组件tabs 滑动）
11. 调用摄像头 （组件uploader 调用摄像头/从相册中选择）
12. 菜谱点赞
13. 消息推送
14. 账单流水
15. .。。

## 路由封装
```
  const routerPath = {
    "login":"/pages/login/login"
  }

  module.exports = {
    // this.$router.push("/index",{path:"/index",query:{}})
    // /index?name=iwen&age=20  query={ name:'iwen',age:20 }   axios  fetch post参数类型 querystring
    push(path,option={}){
      .....
    },
    parse(data){
      ...
      return arr.join("&");
    }
  }
``` 

## Storage信息存储封装
```ruby 
  store.js
``` 


## Request封装
```ruby 
  request.js
  1.基本请求
  2.为了后续获取数据方便，promise处理：fetch  axios基于promise
``` 

## 服务接口封装
```ruby 
  api.js
``` 

## 环境变量封装
```ruby 
  module.exports = {
    Dev:{
      baseApi:""
    },
    Test:{
      baseApi:""
    },
    Prod:{
      baseApi:""
    }
  }
``` 
