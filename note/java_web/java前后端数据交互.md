# 前后端数据交互（Spring）
---
### 数据格式
+ 当前前后端交互的主要格式为json
+ 后端返回数据时spring MVC会自动将java的对象或者字符串转化为json格式放在body里返回给前端
+ 转换规则：将成员变量名当成 JSON 的 键名，将getter方法获取到的值当作 键 对应的数值。

---
### 后端接收前端数据
* 后端有三个接收空间接收前端返回的数据
* url：前端在通过url访问后端资源时可以通过？来携带参数：
* header：通过加@RequestHeader注明字段的参数时请求头传参；
* body: 通过加@RequestBody注明字段参数时body传参。
* 同样后端接收到前端传来的json数据时也会自动将其转化为java对象。
