# ChatGPT-Prompt-Sample-Japanese
ChatGPT の Prompt のサンプルです。

# 注意点
全ては自己責任です。ご利用は十二分に注意をしてください。以下は ChatGPT に限らず情報管理の一般論とも言えますが。

- 機微な情報、機密情報は入力しない
- 出力結果を鵜呑みにしない
- 利用にあたっては、知財・法的な課題を会社・組織の法律の専門家に確認する

# Prompt Engineering の Guide
https://www.promptingguide.ai/jp

# Tool

## 1. Microsoft Copliot (Bing Chat)
https://www.bing.com/

## 2. OpenAI
https://chat.openai.com/chat

## 3. Azure OpenAI Service
https://learn.microsoft.com/ja-jp/azure/cognitive-services/openai/overview

## 4. Prompt Engineering Basic
https://github.com/microsoft/OpenAIWorkshop/tree/main/scenarios/prompt_engineering

# Hello World - はじめの一歩

ChatGPT の基礎的な Prompt です。

# Prompt 

```cmd
### 役割 ###
関西の方として振舞ってください。
```
## 作成途中のものを続けてもらう

ChatGPTに限らずLLMには出力トークン数の制限があります。出力途中で「終わった」という扱いになる事があります。プログラムコードを作成してもらっている際などには、良く遭遇します。

そんな際には、以下のようなPromptを使ってみるといいかもしれません。

```cmd
作業を続けてください。
```

## 自己改善してもらう

`パワハラ プロンプト`という言い方をしている方もいます。
一度、出力結果が思った通りにならない場合、Promptを変更してみることよくあります。その際に、どういう変更をしたらいいのかをChatGPTに考えてもらいます。数回試してもいいかもしれません

このPromptを実行した結果で試した後に、以下を**じっくり考える事**をお勧めします。次回から、もっと短い回数のPromptでご自身の欲しい結果が得られやすくなります。

- どんな改善があったのか?
- なぜその改善をしたのか?

```cmd
プロンプトで設定した目的に対して、作成した出力を60点だとします。
どうやったら100点に改善できますか?100点にするため不足してるものを具体的に列挙してください。100点にする答えを作成してください。
```

参考: ～生成AI業界のトップランナーが語る～ビジネスへのアドオンでおさえるべき知識と最新動向 (オンライン/参加無料)【10/22開催】JDLA緊急企画！:
https://www.youtube.com/live/YX0_GvD0jkE


# 参考

各種Prompt Engineeringの日本語実例集（Zero-CoT、mock、ReAct、ToT、Metacog、Step Back、IEPなど） by @YutaroOgawa2 さん

https://qiita.com/YutaroOgawa2/items/aca32f8fd7d551596cf8

LLMのプロンプト技術まとめ by @fuyu_quant さん

https://qiita.com/fuyu_quant/items/157086987bd1b4e52e80