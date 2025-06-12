# dataiku cloudstack AWSデプロイ関係手順整理

##

## 踏み台サーバへの接続

### 踏み台サーバへの接続準備

### 踏み台サーバへの接続

targetを接続先インスタンスIDに書き換えて、下記を実行してください。

```sh
aws ssm start-session --region ap-northeast-1 --target i-xxxx --document-name AWS-StartPortForwardingSession --parameters "portNumber=3389, localPortNumber=13389"
```
