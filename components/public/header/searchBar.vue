<template>
  <div class="search-panel">
    <el-row class="m-header-searchbar">
      <el-col class="left" :span="3">
        <img
          src="https://s0.meituan.net/bs/fe-web-meituan/fa5f0f0/img/logo.png"
          alt="美团"
        >
      </el-col>
      <el-col class="center" :span="15">
        <div class="wrapper">
          <el-input
            v-model="searchKey"
            placeholder="搜索商家或地点"
            @focus="onFocus"
            @blur="onBlur"
            @input="onInput"
          />
          <el-button class="el-button el-button--primary">
            <i class="el-icon-search" />
          </el-button>
          <dl v-if="isHostPlace" class="hotPlace">
            <dt>热门搜索</dt>
            <dd v-for="(item, index) in hostPlace" :key="index">
              {{ item }}
            </dd>
          </dl>
          <dl v-if="isSearchList" class="searchList">
            <dd v-for="(item, index) in searchList" :key="index">
              {{ item }}
            </dd>
          </dl>
        </div>
        <p class="suggest">
          <a href="#">故宫博物院</a>
          <a href="#">故宫博物院</a>
          <a href="#">故宫博物院</a>
          <a href="#">故宫博物院</a>
          <a href="#">故宫博物院</a>
        </p>
        <ul class="nav">
          <li>
            <nuxt-link to="/" class="takeout">
              美团外卖
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" class="movie">
              猫眼电影
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" class="hotel">
              酒店住宿
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" class="apartment">
              民宿/公寓
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" class="business">
              商家入驻
            </nuxt-link>
          </li>
        </ul>
      </el-col>
      <el-col class="right" :span="6">
        <ul class="security">
          <li>
            <i class="refund" />
            <p class="text">
              随时退
            </p>
          </li>
          <li>
            <i class="single" />
            <p class="text">
              不满意免单
            </p>
          </li>
          <li>
            <i class="overdue" />
            <p class="text">
              过期退
            </p>
          </li>
        </ul>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'SearchBar',
  data () {
    return {
      isFocus: false,
      searchKey: '',
      hostPlace: ['火锅', '烤鱼', '红烧肉'],
      searchList: ['美食', '游玩', '娱乐']
    }
  },
  computed: {
    isHostPlace () {
      return this.isFocus && !this.searchKey
    },
    isSearchList () {
      return this.isFocus && this.searchKey
    }
  },
  methods: {
    onFocus () {
      this.isFocus = true
    },
    onBlur () {
      const self = this
      setTimeout(() => {
        self.isFocus = false
      }, 200)
    },
    onInput (val) {
      this.searchKey = val.trim()
    }
  }
}
</script>
