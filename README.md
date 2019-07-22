# aws-challenge-demo
## aws-challengeとは
「aws-challenge」とは、 **AWS CloudFormation** や **Serverless Framework** を用いて構築されたAWS環境の不具合を見つけ解決しながらAWSに慣れ親しんでもらうことを目的とした学習課題です。

## イントロ 
なぜか動かないLambda!

API Gatewayの設定が悪いのか？

それとも

Lambdaの設定が悪いのか？

今回の指令は「動かないLambdaの謎を解き明かせ」

挑戦者求！

## 今回作成される環境
![aws-challenge-demo-environment](https://user-images.githubusercontent.com/11880332/61526205-f1aafb00-aa54-11e9-90b6-a2dea5b7fd28.png)

* Amazon API Gateway
* AWS Lambda

## 確認事項
* 作成されるLambda関数のhandler.jsには不具合はありません。

## 環境
環境構築に **Serverless Framework** を利用しております。

> https://serverless.com/

```
$sls -v
1.44.1
```

## 環境構築方法
```
$git clone https://github.com/tomonoriminegishi/aws-challenge-demo.git
$cd aws-challenge-demo
$sls deploy -v
```

### パラメータオプション
sls deploy時にパラメータを設定できます。

| パラメータ | デフォルト値 |
----|---- 
| stage | dev |
| region | ap-northeast-1 |
| profile | default |

## 環境撤去方法
```
$cd aws-challenge-demo
$sls remove -v
```


