# mqtt-chat-app-cs

## 開発環境
---
### フロントエンド
- TypeScript
- next.js(react)
  - Hooks API
  - styled-components
  - ESLint
  - prettier
  - storybook

### バックエンド
- C#

### MQTTサーバー
- mosquitto

<br>

## mosquitto動作確認
---

<br>

cmdかシェルを開いてディレクトの移動
```
cd c:\program files\mosquitto
```

MQTT brokerの立ち上げ
```
mosquitto -v
```

別の cmd もしくは shell を立ち上げて<br>
subscriber(データ受信側)
```
mosquitto_sub -d -t TOPICNAME
```

別の cmd もしくは shell を立ち上げて<br>
publisher(データ送信側)
```
mosquitto_pub -d -t TOPICNAME -m "message"
```

<br>

## 参考文献
---
<br>
WindowsでMQTT (mosquitto) | Program Resource<br>
https://programresource.net/2020/03/28/3204.html