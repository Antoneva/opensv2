
<h1 align="center"> 免责声明 </h1>


<p align="center">
只面向海外华人用户且仅供科研学习之用，切勿用于其他用途
<br>
中国居民请自觉关闭本项目并24小时之内删掉与本项目相关的一切内容，否则出现一切问题，项目作者概不负责
</p>
<hr>



# v2ray 部署在 openshift starter
openshift: 内存设置为256M，每 project 可配置 4 Pods。

环境变量： CONFIG_JSON（配置）
{
  "log": {
    "loglevel": "warning"
  },
  "inbound": {
    "protocol": "vmess",
    "port": 8080,
    "settings": {
      "clients": [
        {
          "id": "UUID",
          "alterId": 64,
          "security": "chacha20-poly1305"
        }
      ]
    },
    "streamSettings": {
      "network": "ws"
    }
  },
  "inboundDetour": [],
  "outbound": {
    "protocol": "freedom",
   "settings": {}
  }
}



youtube频道：https://www.youtube.com/channel/UClceV39J1Z_9D4_mHkBZrMg

