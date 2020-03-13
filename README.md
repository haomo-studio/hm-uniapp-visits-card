> 官网: [https://haomo-tech.com](https://haomo-tech.com)

> 作者: 毫末科技

> 邮箱: hxg@haomo-studio.com

## 预览

![预览图片](http://downloads.haomo-tech.com/uniapp/hm-visits-card.png)

[在线效果预览](http://template.uniapp.haomo-tech.com/pages/haomo/test-component/hm-visits-card)

更多毫末科技的uni-app跨端模板，请见[毫末科技uni-app跨端模板](https://haomo-tech.com/sale.html)

## 技术支持

* [uni-app插件市场](https://ext.dcloud.net.cn/plugin?id=1424)

* [npm包](https://www.npmjs.com/package/hm-uniapp-visits-card)

* [github地址](https://github.com/haomo-studio/hm-uniapp-visits-card)

* [gitee地址](https://gitee.com/haomo/hm-uniapp-visits-card)

毫末科技将长期迭代本组件。需要技术支持，请进钉钉群：

<img width="250" src="http://downloads.haomo-tech.com/%E6%AF%AB%E6%9C%ABuniapp%E7%BB%84%E4%BB%B6%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81.jpg">

## 概述

毫末uni-app毫末访问量卡片组件。支持H5/小程序(微信、支付宝、头条、百度、QQ)/App；组件可自适应各种屏幕大小的手机。

## 使用

请使用HBuilderX导入组件。

在script中引用：

```javascript
import HmNewsCard from '@/components/hm-visits-card/index.vue'
export default {
    components: { HmVisitsCard }
}
```

在template中使用：

```html
<template>
  <div class="test-component">
    <hm-visits-card :options="options"></hm-visits-card>
  </div>
</template>
<script>
import HmVisitsCard from '@/components/hm-components/hm-visits-card/index.vue'

export default {
  components: { HmVisitsCard },
  data() {
    return {
     options: {
         text: '日常访问',
          img:
            'staticimg_24227_0_1.png',
          jiantouimg:
            '/static/hm-visits-card/images/img_24227_0_2.png',
          num: '+3.49%',
          nums: '178080',
          unit: '个',
          shopLogo:
            '/static/hm-visits-card/images/img_24227_0_0.png'
        }
    };
  },
  methods: {
    onClick: function(e) {
      console.log('onClick');
    }
  }
};
</script>
<style>
</style>
```

## 属性说明

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| options        | Object  | -      | 卡片属性                                                                   |

options对象各个属性说明如下：

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| text        | String  | -      | 标题文字                                                                   |
| img        | String  | -      | 图片                                                                   |
| jiantouimg        | String  | -      | 图片                                                                   |
| num        | String  | -      | 增长百分比                                                                   |
| nums        | String  | -      | 增长量                                                                   |
| unit        | String  | -      | 单位                                                                   |
| shopLogo        | String  | -      | 图片                                                                   |

## 事件说明

| 事件称名   | 事件说明           | 返回参数 |
|----------|--------------------|----------|
| @click   | 点击 Card 触发事件 | -        |

## 更新日志

### 0.0.1(2020-03-13)

* 完成第一个版本
