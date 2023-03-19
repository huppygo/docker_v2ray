# 基于另一个项目v2ray_client做的docker封装

# 拉取镜像

docker pull huppygo/open:v2rayclientv1.0

#拉取项目文件

git clone https://github.com/huppygo/docker_v2ray.git

docker run -d --restart=always --name v2ray \
  -v /修改成你的目录/v2ray_client/config/v2ray/:/etc/v2ray \
  -v /修改成你的目录/v2ray_client/app.db:/home/NoOne-hub/v2ray/app.db \
  -p 10808:10808 -p 10809:10809 -p 8000:8000 v2ray

#默认账号:NoOne-hub

#默认密码:1234567890

#部署完成后可以直接访问http://localhost:8000  记得防火墙开启端口

