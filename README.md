# aws-challenge-demo
なぜか動かないLambda!今回の指令は「動かないLambdaを動かす！」挑戦者求！

# 環境
この問題の環境構築に *Serverless Framework* を利用しております。

```
$sls -v
1.44.1
```

# 環境構築方法

```
$git clone https://github.com/tomonoriminegishi/aws-challenge-demo.git
$cd aws-challenge-demo
$sls deploy
```

## パラメータオプション
sls deploy時にパラメータを設定できます。

| パラメータ | デフォルト値 |
----|---- 
| stage | dev |
| region | ap-northeast-1 |
| profile | default |

# 今回作成される環境
![aws-challenge-demo-environment](https://user-images.githubusercontent.com/11880332/61526205-f1aafb00-aa54-11e9-90b6-a2dea5b7fd28.png)

* Amazon API Gateway
* AWS Lambda

# 確認事項
* 作成されるLambda関数のhandler.jsには不具合はありません。
