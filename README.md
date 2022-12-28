# Hideipnetwork Server

hideipnetwork was developed to evade censorship on the web

**`Demo`**：[https://hideip.network](https://hideip.network)

---

## Quickstart  |  [中文教程](https://github.com/Hideipnetwork/hideipnetwork-web/wiki/hnet-web-nodejs%E7%89%88%E6%9C%AC%E6%95%99%E7%A8%8B)

* *Need install Node.js 16+*

```
git clone https://github.com/Hideipnetwork/hideipnetwork-web.git

cd hideipnetwork-web

npm i && npm run start
```

**Besides that, you have to deploy api（if you need set password）** [hidwipnetwork-admin](https://github.com/Hideipnetwork/hideipnetwork-admin) !!!

## Nginx configuration

```nginx notranslate position-relative overflow-auto
location / {
  proxy_busy_buffers_size  512k;
  proxy_buffers  4 512k;
  proxy_buffer_size  256k;
  proxy_pass http://localhost:3000;
  proxy_http_version 1.1;
  proxy_set_header Upgrade $http_upgrade;
  proxy_set_header Connection 'Upgrade';
  proxy_set_header X-Real-IP $remote_addr;
  proxy_set_header X-Forwarded-Host $host:$server_port;
  proxy_set_header X-Forwarded-Server $host;
  proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
  proxy_set_header Host $host;
}
```

## Donate(TRC20)

![](https://alis.pages.dev/file/7aa0321085f5e963eae40.png)

TQVFVa7Hmbycp1q3r3tUdTL9NzAR1XAy9E

## contact

![](https://store.heytapimage.com/cdo-portal/feedback/202207/02/b705611e231f230f2fec150f35221c0b.png)
