## 说明

- 基于最新PHP7.1-cli版本
- 使用swoole2.X最新稳定版本构建
- 已安装 ["GD", "mcrypt", "iconv", "pdo_mysql", "dom", "xml", "curl", "swoole"]等PHP扩展
- 已开启["coroutine", "openssl", "http2", "async-redis", "mysqlnd"]扩展
- 纯环境 , 无任何php代码
- 默认中国上海时区

---

- use swoole 2.* latest stable version
- PHP extension installed: ["GD", "mcrypt", "iconv", "pdo_mysql", "dom", "xml", "curl", "swoole"]
- enable ["coroutine", "openssl", "http2", "async-redis", "mysqlnd"]
- this container has no PHP code or framework included
- Asia/Shanghai timezone default (you can remove it on first RUN line)

## Usage

```Bash
docker run -d --name=swoole \
 -v /workdir:/workdir \
 -p 9501:9501 \
 twosee/swoole-coroutine \
 php /app/server.php start
```