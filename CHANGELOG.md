---
title: 更新日志
docClass: timeline
toc: false
spline: explain
---
## 🌈 0.8.6 `2022-05-30` 
### 🚀 Features
- `Indexes`: 新增 Indexes 组件 @ruige24601 ([#117](https://github.com/Tencent/tdesign-mobile-vue/pull/117))
- `ActionSheet`: 新增 ActionSheet 组件 @Dengzygx ([#121](https://github.com/Tencent/tdesign-mobile-vue/pull/121))
- `Icon`: 更新图标 新增`file-icon`图标 调整`file-excel`、`file-pdf`、`file-powerpoint`、`file-unknown`、`file-word`和`star-filled`图标的绘制路径 @uyarn ([#111](https://github.com/Tencent/tdesign-mobile-vue/pull/111))
### 🐞 Bug Fixes
- `Textarea`: 修复label不生效问题；样式优化 @anlyyao ([#107](https://github.com/Tencent/tdesign-mobile-vue/pull/107))
- `Badge`: 修复组件设置 color 属性无效问题 @Calvest ([#125](https://github.com/Tencent/tdesign-mobile-vue/pull/125))
- `Swiper`: 支持通过修改loop值关闭循环 @MarvenGong ([#108](https://github.com/Tencent/tdesign-mobile-vue/pull/108))
### 🚧 Others
- Refactor: 将 mask 重命名为 overlay @LeeJim ([#113](https://github.com/Tencent/tdesign-mobile-vue/pull/113))
- Refactor: 重构Progress组件，Api更新 @anlyyao ([#116](https://github.com/Tencent/tdesign-mobile-vue/pull/116))
- Refactor: 重构 Slider 组件 @LeeJim ([#115](https://github.com/Tencent/tdesign-mobile-vue/pull/115))
- Refactor: 重构 NoticeBar 组件 @xia7187 ([#99](https://github.com/Tencent/tdesign-mobile-vue/pull/99))
- feat: 站点支持搜索 @HQ-Lin ([#120](https://github.com/Tencent/tdesign-mobile-vue/pull/120))

## 0.8.5 `2022-04-29`


### Bug Fixes

* **Indexes:** 暂时从菜单栏中移除
* **Picker:** 修复组件demo点击取消,无法收起蒙层问题
* **DateTimePicker:** 修复组件传参错误问题、修复组件无法触发change事件问题
* **Textarea:** 修复组件类名错误问题

### Features
* **Icon:** 完善组件文档

## 0.8.4 `2022-04-15`


### Bug Fixes

* **Swiper:** 修复动态绑定时出错问题
* **List:** 修复组件demo代码运行出错的问题
* **Input:** compositionend优化


### Features

* **Tabs:** 新增stickyProps，支持滚动到顶部时自动吸顶
* **PullDownRefresh:** loadingBarHeight属性支持string类型，代码优化

## 0.8.2 `2022-04-08`


### Bug Fixes
* **tabs:** label支持动态修改，以及新增支持slot的方式 
* **popup:** 修复teleport失效问题


## 0.8.1 `2022-04-02`

### Bug Fixes

* **count-down:** 单位样式bug修复、倒计时加入fps获取
* **swiper:** 快速滑动导致卡住问题
* **picker:** 组件demo修复
* **swipe-cell:** 修改组件示例，和demo保持一致


### Features

* 加入ci拼写检查报错
* 支持历史版本跳转
* **dropdown-menu:** 更新组件的模板类型处理

## 0.8.0 `(2022-03-17)`


### Bug Fixes
* **dropdown-menu:** 移除冗余的dom结构 ecba97f
* **search:** 修复样式丢失问题, close #29 ac1dd2a, closes #29
* **input** 修复输入框样式丢失问题
* **grid** 修复grid-item样式丢失问题


### Features
* 新增pull-down-refresh组件 6f1c8a7


## 0.7.0 `(2022-03-14)`

### BREAKING CHANGES

* **count-down**支持主题和大小 3f0a5e5

### Bug Fixes

* **dialog**弹出框蒙层点击是否关闭修复 & provide暴露$dialog, close #12 11092af, closes #12
* 修复Badge导入类型 d4f8da6

### Features

* 新增BackTop组件 fb61e74

## 0.6.2 `(2022-03-03)`

### Bug Fixes

* 修复缺失的组件引用 `bug #149`
* **dialog:** buttons layout 92944ee
* **steps** 设计修改样式对齐 38ca336
* **swiper:** 非空Props的处理
* **tabbar:** 调整demo默认值使用
* **input** modelValue绑定丢失的问题 `bug #151`

## 0.6.1 `(2022-02-28)`


### Bug Fixes

* **avatar:** 移除完全一样的逻辑实现
* **demo:** 修复demo展示问题&移除indexes
* **picker:** 修复picker的错误
* **steps** steps只读demo不可点击问题修复
* **swiper:** 修复类型错误
* **tabs:** 移除顶部transform
* **toast:** 修复遮罩禁止滑动不生效的问题

### Features

* 新增 stackblitz 支持
* 引入vueuse, 优化代码逻辑
* 优化图片懒加载方案
* 新增Image、Sticky、Skeleton、Grid、List、Loading组件
* 引入useDefault处理受控和非受控逻辑
* 引入useEmitEvent处理事件逻辑:stepper, image
* 移除mapprops高阶组件
* 处理props对于可空类型的判断ts提示问题
* Stepper增加overlimit支持

### BREAKING CHANGES

* **datetimepicker:** 改变API由position为placement

## 0.5.0 `(2022-01-23)`

### Bug Fixes

* **tag:** 更新tag样式light-outline 1e051bd
* **picker:** 修复默认值非第一个时的滚动错误 1ff7183
* **avatar:** 修复size和dot的支持 class 57fe446
* **cell:** icon对齐的问题 7c71689
* **checkbox:** 组件对齐的问题 78f5bb0
* **dialog:** 修复dialog插件类型错误 f7983d7
* **dropdown-menu:** 修复单选项目 update:value 失效的问题 68e62bd, 修复一些特殊场景出现的问题 ffc2f4e
* **input:** 修复点击事件丢失问题 31f1a39
* **radio:** 修复radio的文本点击事件丢失问题 3664b5f
* **rate:** 修复视觉走查 b7bd53a
* **swiper:** 添加圆角支持 69aa8e5

### Features

* 完善avatar组件
* 完善picker默认值以及demo fa1983a
* 添加useDefault（支持受控和非受控逻辑）支持setInnerValue  dc8262d
* checkbox and check-group结构调整 fe53611
* picker-item的value变化时，picker及时更新 5b12841

## 0.4.1 `(2022-01-06)`

### Bug Fixes

* Swiper: 修复Swiper宽度计算问题 cc2d012
* typo e25903a

### Features

* Avatar: 添加Avatar组件
* 更新BEM规范 7c59f2b,5637f7e
* 迁移 md & 优化细节 e4c28fa,048a9aa,799fc08
* 添加 codesandbox 5fea71d, e93e416

## 0.4.0 `(2021-12-27)`

### Features

* **switch:** use emitEvent ([1700a72](http:///tdesign-mobile-vue/commits/1700a722c896c43658512de36b7235f6655981ae))
* 补充 package.json 信息，使用 cli 处理发布日志 ([eb4fa42](http:///tdesign-mobile-vue/commits/eb4fa42df755749bfbd48f9cf9dc591f8bb00b49))
* 调整 common & types目录 ([227e7dd](http:///tdesign-mobile-vue/commits/227e7dd2c67448d6c30cf325c72ae6967d63779c))
* 调整贡献者名单位置 ([c92c5c9](http:///tdesign-mobile-vue/commits/c92c5c9b63a6a4e60bf093c28e66dc550d1bfcd7))
* 新增 Countdown、 Swiper组件

### BREAKING CHANGES

* 对齐已发布组件的API能力
