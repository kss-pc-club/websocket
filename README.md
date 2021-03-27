# WebSocket
HerokuでデプロイするためのWebsocketのリポジトリ。<br>
このHerokuプロジェクトへのアクセス権がほしい方は、Slackで`Asa`まで連絡ください。

wss://kss-pc-club-websocket.herokuapp.com/

## 使い方
```js
const websocket = new WebSocket('wss://kss-pc-club-websocket.herokuapp.com/[プロジェクト名]/aaa');
websocket.addEventListener('open',()=>{
  console.log('接続しました');
})
websocket.addEventListener('message',msg=>{
  console.log(`メッセージ: ${msg.data}`);
})
websocket.addEventListener('close',()=>{
  console.log('切断しました')
})
websocket.addEventListener('error',()=>{
  console.log('エラーが発生しました')
})
```

## サンプルページ
https://kss-pc-club-websocket.herokuapp.com/(任意のファイル名)

## 開発方法
1. `git clone https://github.com/kss-pc-club/websocket.git`
2. `npm install`
3. `npm start`

## 必要環境
[SECURITY.md](./SECURITY.md) を見てください

## 行動規範
[CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md) を見てください

## 貢献したい方
[CONTRIBUTING.md](./CONTRIBUTING.md) を見てください

## LICENSE
MIT License. [LICENSE file](./LICENSE) for more information.
