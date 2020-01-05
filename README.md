1）编码测试
npm run dev
访问:http://localhost:8082

2）项目描述
包括商家、商品、购物车、用户等子模块
使用Vue全家桶 ES6 等
前台应用技术架构为: vue + vuex + vue-router
后台应用技术架构为: Node + Express + Mongodb + Mongoose

路由组件 src/pages
一般组件 src/components

Msite（首页）：HeaderTop 头部组件、FooterGuide 底部组件、ShopList 商家列表、Stars 星级
Search（搜索）：HeaderTop
Profile（个人中心）：HeaderTop
Order（订单）：HeaderTop
Login（登录）：AlertTip（提示框）
Shop（商品详情页）：ShopHeader 头部、Stars
  --ShopGoods（商品列表）：CartControl（加减商品）、Food（商品详情）、ShopCart（底部的购物车）
  --ShopRatings（商家评价）：Stars
  --ShopInfo（商家信息）
