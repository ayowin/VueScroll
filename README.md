# VueScroll

#### 介绍
vue项目的上拉刷新，下拉加载组件，已封装独立的控件。

#### 使用方法

* 可将Scroll.vue复制到您的vue项目，到任何一个vue文件中，将以下示例代码复制到相应的模块即可试看效果。
* 参考HomeMobile.vue代码。

```vue
<Scroll class="scroll" 
        downPullBackgroundColor="ghostwhite" 
        @upPullEvent="onScrollUpPullEvent" 
        @downPullEvent="onScrollDownPullEvent">
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
    <h1>dfasdfasdfa</h1>
</Scroll>

<script>
	import Scroll from "./Scroll.vue"
	export default {
		components: {
			Scroll
		},
		methods: {
			onScrollUpPullEvent() {
				console.log("on scroll upPullEvent");
			},
			onScrollDownPullEvent() {
				console.log("on scroll down refresh");
			}
		}
	}
</script>
```

#### 属性说明

```vue
props: [
			'downPullHintText', // 下拉提示文本
			'downPullReleaseText', // 下拉释放文本
			'downPullLoadText', // 下拉加载文本
			'downPullBackgroundColor', // 下拉背景颜色
			'downPullFontColor', // 下拉字体颜色
			'downPullFontSize' // 下拉字体大小
		]
```

#### 事件说明

```vue
@upPullEvent // 上拉事件：滚到到最底会触发本事件
@downPullEvent // 下拉时间：下拉即可触发本事件
```

