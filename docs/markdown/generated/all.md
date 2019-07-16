# Api Documentation


<a name="overview"></a>
## 概览
Api Documentation


### 版本信息
*版本* : 1.0


### 许可信息
*许可证* : Apache 2.0  
*许可网址* : http://www.apache.org/licenses/LICENSE-2.0  
*服务条款* : urn:tos


### URI scheme
*域名* : localhost:8080  
*基础路径* : /


### 标签

* demo-controller : 用户接口




<a name="paths"></a>
## 资源

<a name="demo-controller_resource"></a>
### Demo-controller
用户接口


<a name="createuserusingpost"></a>
#### 新增用户
```
POST /demoController/createUser
```


##### 说明
新增注册


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Body**|**user**  <br>*必填*|user|[User](#user)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[ResObject](#resobject)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/demoController/createUser
```


###### 请求 body
```
json :
{
  "email" : "string",
  "password" : "string",
  "userId" : "string",
  "userName" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "code" : 0,
  "data" : "object",
  "desc" : "string"
}
```


<a name="deleteuserusingdelete"></a>
#### 删除用户
```
DELETE /demoController/deleteUser
```


##### 说明
删除用户


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Query**|**userId**  <br>*必填*|用户标识|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[ResObject](#resobject)|
|**204**|No Content|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/demoController/deleteUser
```


###### 请求 query
```
json :
{
  "userId" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "code" : 0,
  "data" : "object",
  "desc" : "string"
}
```


<a name="queryuserusingget"></a>
#### 查询用户
```
GET /demoController/queryUser
```


##### 说明
查询用户


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Query**|**userId**  <br>*必填*|用户标识|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[ResObject](#resobject)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/demoController/queryUser
```


###### 请求 query
```
json :
{
  "userId" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "code" : 0,
  "data" : "object",
  "desc" : "string"
}
```


<a name="updateuserusingpost"></a>
#### 修改用户
```
POST /demoController/updateUser
```


##### 说明
修改用户


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Body**|**user**  <br>*必填*|user|[User](#user)|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[ResObject](#resobject)|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/demoController/updateUser
```


###### 请求 body
```
json :
{
  "email" : "string",
  "password" : "string",
  "userId" : "string",
  "userName" : "string"
}
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "code" : 0,
  "data" : "object",
  "desc" : "string"
}
```




<a name="definitions"></a>
## 定义

<a name="resobject"></a>
### ResObject

|名称|说明|类型|
|---|---|---|
|**code**  <br>*可选*|**样例** : `0`|integer (int32)|
|**data**  <br>*可选*|**样例** : `"object"`|object|
|**desc**  <br>*可选*|**样例** : `"string"`|string|


<a name="user"></a>
### User

|名称|说明|类型|
|---|---|---|
|**email**  <br>*可选*|**样例** : `"string"`|string|
|**password**  <br>*可选*|**样例** : `"string"`|string|
|**userId**  <br>*可选*|**样例** : `"string"`|string|
|**userName**  <br>*可选*|**样例** : `"string"`|string|





