### frp反代 + caddy 自动 https docker 服务

##### 1.先 clone
`git clone https://github.com/yybawang/frp-caddy.git`
##### 2.更改三个文件配置，记得服务器要在安全组里加白端口
```shell
./caddy/caddy/Caddyfile
./frp/frpc.toml
./frp/frps.toml
```
##### 3.服务器端启用服务
`sudo docker compose up -d caddy frps`

#### 4.本地端启用服务
`sudo docker compose up -d frpc`
