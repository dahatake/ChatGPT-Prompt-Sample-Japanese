# 観光Webアプリのプロトタイプ開発

ChatGPT あるいは Azure OpenAI Services の PlayGround などで行います。

Azure OpenAI Services の PlayGround:

https://learn.microsoft.com/ja-jp/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cpython&pivots=programming-language-studio

プロトタイプの実装では、利用する製品・サービス・テクノロジーを決めます。

ここでは、サーバー側の処理は Microsoft Azure で。Webアプリは Vue.JS で行います。これはご自身の好みで😊

Vue.JS 入門:

https://learn.microsoft.com/ja-jp/training/paths/vue-first-steps/


# 1. 要件定義

## 1.1 作りたいビジネスシナリオを決める

テーマ: 観光発掘

ターゲットユーザー:

- 郡山に来た人がスムーズに過ごせるように
- ペルソナ: 私 @dahatake

@dahatake の悩み:

- 美味しいごはんを食べたい
- ステキな景色をみたい
- 移動手段を何とかしたい
- 支払い方法を簡略化したい

# 2. 要件を定義する

ドキュメントは作成しません。あくまで、チームメンバー内で共有できればいいという最低限のものを。
ChatGPT を使います。

## 2.1.　要件定義

Prompt:
```cmd
### 役割 ###
あなたは世界最高峰のソフトウェアエンジニアです。

### 指示 ###
以下の要件に沿ったユースケースを考えてください。

### 要件 ###
- 福島県郡山市の観光をサポートするWebアプリケーションを作成したい
- 美味しいごはんを食べたい
- ステキな景色をみたい
- 移動手段を何とかしたい
- 支払い方法を簡略化したい
```
## 2.2. データモデル作成

Prompt:
```cmd
それでは、これらのユースケースをシステムとして実現するために、どの様なデータモデルが考えられますか? Mermaid live editor のER図で作成してください。
```

Prompt:

```cmd
ユーザーが操作する画面の画面遷移図を Mermaid live editor の書式で作成してください。
```

## 3. プロトタイプ作成

### 3.1. データモデル

Promot:
```cmd
データモデルを Vue.js 用に出力してください
```

### 3.2. 画面

Promot:
```cmd
Vue.js と HTML で画面を作成してください。

画面: ###
- ホーム画面
- 観光地検索
- 観光地一覧表示
- 観光地詳細
###
```

### 3.3. API

```cmd
API を NodeJS で作成してください。
```

```cmd
APIに以下の機能を加えてください。

機能:###
- Azure Functions でホスティング
- データは Azure Cosmos DB に保存する
###
```

```cmd
各Vue.jsから、Azure Functions 上でホスティングされているAPIを呼び出すコードを作成してください。
```

# 4. メモ
外部サービスの呼び出しをしたいです。Bing Chat や Google Search などで、郡山の観光データベースを探します。

Copilot (旧Bing Chat)

Prompt:
```cmd
福島県郡山市の観光名所をAPIとして公開しているサービスはありますか?
```
残念ながらありませんでした。

ですが、以下のサイトは見つかりました。となれば、これをデータベース化する必要がありますね。

https://www.kanko-koriyama.gr.jp/

ここでは残念ですが、幾つかを手作業で入手することにします。Excel に搭載されている Power Query を使って、ローカルにCSVとして出力します。