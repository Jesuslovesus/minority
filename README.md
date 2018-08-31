## 接口文档

# 数据展示接口（共 个）

## `GET` bread/v1/provinces `获取所有省份列表`

### 传参说明
字段|作用|默认值|说明|数据类型
:---		|:--		|:--		|:--		|:--
type	|根据不同的值返回相应的参数	|`1`or`null`<br>无此参数默认返回所有省份		| (暂时不需要，先由前端自行分组，后期升级)<br>`1`：返回数据库中所有的省份列表；<br>`2`：返回所有正式发布的省份；<br>`3`：返回还未正式发布的省份 | number

### 返回值
> 根据参数返回所有省份的基本信息列表

请求类型|作用|默认值|说明|数据格式
:---		|:--		|:--		|:--		|:--
id	|省份唯一标识	|		|  |number
lable|省份显示名称|
name|省份拼音|
value|省份标志（暂同name值）
bg	|省份主题色	   |		|  |string
img	|省份主题图片	|		|图片链接地址	|url
show|是否已正式发布|false|`false`：还未录入信息;<br>`true`：已正式记录发布


### 返回数据

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
## `GET` bread/v1/provinces/{id} `获取指定省份详细信息`