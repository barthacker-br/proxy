[English](README.md) | 简体中文

# proxy
HTTP 请求代理，CORS 跨域请求，HTTPS 支持

### 作用
- 支持跨域请求（转换不支持跨域请求的接口），可直接发起 ajax、fetch
- 支持 HTTPS（解决远程数据接口不支持 HTTPS）

### 使用
- Host/{URL}
- <https://proxy.zme.ink/api.github.com>
- <https://proxy.zme.ink/http://nginx.org/download/nginx-1.20.1.zip>

```js
// 拷贝到控制台运行

var $url = "wthrcdn.etouch.cn/weather_mini?citykey=101040100";
fetch("https://proxy.zme.ink/" + $url).then(x => x.json()).then(console.log)
```

### 运行
```
npm start   # 启动

# node app.js
# PORT=8888 node app.js
```

### 源码
- Fork：<https://github.com/Rob--W/cors-anywhere>
- <https://github.com/netnr/proxy>