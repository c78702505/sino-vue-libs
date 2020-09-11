# 培训组件库

[查看在线文档](https://c78702505.github.io/sino-vue-libs/)

## 安装
```
npm install sino-vue-libs -S
```

### 快速上手

-  main.js 中引入 sino-vue-libs

```
// main.js
import SinoComponents from 'sino-vue-libs'
Vue.use(SinoComponents)
// or
import {
	SinoImage,
	SinoAvatar
	// ...
} from 'sino-vue-libs'
Vue.component(SinoImage.name, SinoImage)
Vue.component(SinoAvatar.name, SinoAvatar)
```

- 具体调用

```
<template>
	<sino-image />
	<sino-card-lg-words :num=2></sino-card-lg-words>
	<sino-card-img-words-item v-bind="imgItem"></sino-card-img-words-item>
	...
</template>
<script>
	export default {
		data:{
			imgItem:{
				layout: 'row',
				title: '可视化布局',
				date: '2020-10-10',
				zanNum: '10',
				author: '罗老师',
				// talkNum:'200',
				// cangNum:'100',
				tags:[
					{text: '热门',type: 'error'},
					{text: '在学',type: 'success'},
				]
			}
		}
	}
</script>
```

[查看在线文档](https://c78702505.github.io/sino-vue-libs/)

## LICENSE
[MIT](LICENSE)
