<template>
  <div class="m-nav">
    <ul class="nav">
      <li class="list">
        <nuxt-link to="/my">
          我的美团
        </nuxt-link>
        <dl>
          <dd>
            <nuxt-link to="/myOrder">
              我的订单
            </nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/myOrder">
              我的收藏
            </nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/myOrder">
              抵用券
            </nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/myOrder">
              账户设置
            </nuxt-link>
          </dd>
        </dl>
      </li>
      <li>手机APP</li>
      <li class="list bd">
        <nuxt-link to="/center">
          商家中心
        </nuxt-link>
        <dl>
          <dd>
            <nuxt-link to="/userCenter">
              商家中心
            </nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/coop">
              我想合作
            </nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/wap">
              手机免费开店
            </nuxt-link>
          </dd>
          <dd>
            <nuxt-link to="/kaipiao">
              商家申请开票
            </nuxt-link>
          </dd>
        </dl>
      </li>
      <li class="list site">
        <nuxt-link to="/site">
          网站导航
        </nuxt-link>
        <div class="subContainer">
          <dl class="hotel">
            <dt>酒店住宿</dt>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
            <dd>热门酒店</dd>
          </dl>
          <dl class="food">
            <dt>吃美食</dt>
            <dd>烤鱼</dd>
            <dd>特色小吃</dd>
            <dd>烧烤</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
          </dl>
          <dl class="movie">
            <dt>看电影</dt>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
            <dd>热映电影</dd>
          </dl>
          <dl class="app">
            <dt>手机应用</dt>
            <dd>
              <a href="#">
                <img src="http://s0.meituan.net/bs/fe-web-meituan/2d53095/img/appicons/meituan.png" alt="美团APP">
              </a>
            </dd>
            <dd>
              <a href="#">
                <img src="https://s1.meituan.net/bs/fe-web-meituan/404d350/img/appicons/waimai.png" alt="外卖APP">
              </a>
            </dd>
            <dd>
              <a href="#">
                <img src="https://p0.meituan.net/travelcube/162c3308d9622f6d9cfaa49e60be4dca8573.png" alt="民宿APP">
              </a>
            </dd>
            <dd>
              <a href="#">
                <img src="https://s1.meituan.net/bs/fe-web-meituan/404d350/img/appicons/dianping.png" alt="点评APP">
              </a>
            </dd>
            <dd>
              <a href="#">
                <img src="https://s1.meituan.net/bs/fe-web-meituan/404d350/img/appicons/maoyan.png" alt="猫眼APP">
              </a>
            </dd>
          </dl>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Nav'
}
</script>

<style lang="scss">
</style>
