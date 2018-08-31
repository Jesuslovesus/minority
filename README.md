## 登录 Jesuslovesus.github.io 即可访问

### 2018.08.02 构建，将持续更新

## 技术栈

html5

css3

js

elementUI

vue 全家桶

webpack


## 接口文档

### `GET` bread/v1/provinces `请求所有省份的列表`

#### 传参说明
无

#### 返回值
* 返回所有省份的列表

请求类型|类型|默认值|说明|数据格式
:---		|:--		|:--		|:--		|:--
id	|省份唯一标识	|		|  |number
lable|省份显示名称|
name|省份拼音|
value|省份标志（暂同name值）
bg	|省份主题色	   |		|  |string
img	|省份主题图片	|		|图片链接地址	|url
show|是否已正式发布|false|`false`:还未录入信息`true`:已正式记录发布


#### 返回数据

```
[
	{
		"img": "/static/media/bread/img/yunnan.jpg", 
		"bg": "blue", 
		"id": 1, 
		"show": true, 
		"name": "yunnan", 
		"value" "yunnan"
		"label": "云南"
	},
	{
		"img": "/static/media/img/sichuan.jpg", 
		"bg": "blue", 
		"id": 2, 
		"show": true, 
		"name": "sichuan", 
		"value": "sichuan", 
		"label": "四川"
	}
]

```