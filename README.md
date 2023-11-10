# ChatGPT-Prompt-Sample-Japanese
ChatGPT の Prompt のサンプルです。

# 注意点
全ては自己責任です。ご利用は十二分に注意をしてください。

- 機微な情報、機密情報は入力しない
- 出力結果を鵜呑みにしない
- 利用にあたっては、知財・法的な課題を法律の専門家に確認する

# Prompt Engineering の Guide
https://www.promptingguide.ai/jp

# Tool

## 1. Bing Chat
https://www.bing.com/

## 2. OpenAI
https://chat.openai.com/chat

## 3. Azure OpenAI Service
https://learn.microsoft.com/ja-jp/azure/cognitive-services/openai/overview

## 4. Prompt Engineering Basic
https://github.com/microsoft/OpenAIWorkshop/tree/main/scenarios/prompt_engineering

# Hello World - はじめの一歩

ChatGPT の基礎的な Prompt です。

# Promot 

```cmd
### 役割 ###
関西の方として振舞ってください。
```

以下は Bing Chat で

```cmd
### 指示 ###
昨日最も視聴率の良かったテレビ番組は何ですか?
```

```cmd
### 指示 ###
昨日最も視聴率の良かったテレビ番組は何ですか?分からない場合は、「分かりません」と出力してください。
```

以下は ChatGPT で。計算は苦手なので、おススメはしません😊 Excel 駆使してください😊

```cmd
### 役割 ###
ファイナンシャルプランナーとして振舞ってください。

### 指示 ###
住宅ローンを組みます。5,000万円を、年率 0.85% で 35年で返金をします。初年度の初月の支払い金額はいくらですか?
```

```cmd
### 指示 ###
住宅ローンを組みます。5,000万円を、年率 0.85% で 35年で返金をします。初年度の初月の支払い金額はいくらですか?算出過程が分かるように段階的に記述してください。
```

```cmd
### 指示 ###
住宅ローンを組みます。5,000万円を、年率 0.85% で 35年で返金をします。初年度の初月の支払い金額はいくらですか?算出過程が分かるように段階的に記述してください。幼稚園児でも分かるように説明をしてください。
```

```cmd
イベントセッションのスクリプトを作って
```

```cmd
Tweet を作って
```

# GPT の思考の方向性を調整する

人にするようなアドバイスをすると、期待した出力結果に近づきやすくなる

CoT (Chain of Thoght) の例:

```cmd
ステップバイステップで考えてください。
```

もう一つ:
https://arxiv.org/abs/2309.03409

```cmd
深呼吸をして、この問題に一歩ずつ取り組んでください。
```


制限の例:

```cmd
目的が達成できない場合は、不足している情報を、質問してください。
```

思考の方向性を定義:

```cmd
【クリエイティブな発想が欲しい場面】
- 非線形思考
- 多角的思考
- 型破りな思考
- アウトオブザボックス思考
- 発散思考
- 閃き思考
- 逆説思考
- 冒険的思考
- 左脳思考
- 右脳思考

【問題解決に特化した場面】
- 分析思考
- 全体論的思考
- 抽象化思考
- 問題解決思考
- システム思考
- 仮説思考
- プロセス思考
- IF思考

【組織やビジネスでの戦略的思考が必要な場面】
- イシュードリブン思考
- レバレッジ思考
- 戦略思考
- 価値創造思考
- スタートアップ思考
- DX思考

【詳細な分析や論理的な議論が必要な場面】
- 論点思考
- クリティカルシンキング
- 批判的思考
- 水平思考
- 垂直思考
- 演繹的思考
- 帰納的思考

【コミュニケーションや表現が必要な場面】
- デザイン思考
- ビジュアル思考
- 言語思考
- アート思考
- 図解思考
- コンテキスト思考
- アナロジー思考
```

source:
https://twitter.com/ctgptlb/status/1710062428778537337?s=43&t=C4VBAwZGDwmbZHLBoG98OA


# 参考

各種Prompt Engineeringの日本語実例集（Zero-CoT、mock、ReAct、ToT、Metacog、Step Back、IEPなど） by @YutaroOgawa2 さん

https://qiita.com/YutaroOgawa2/items/aca32f8fd7d551596cf8

LLMのプロンプト技術まとめ by @fuyu_quant さん

https://qiita.com/fuyu_quant/items/157086987bd1b4e52e80