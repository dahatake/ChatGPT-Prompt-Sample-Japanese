# Workshop

今抱えているお仕事や学業など、自分の関心事に応じて、それぞれの Prompt を置き換えてください。


# 1. 基本動作

## 1.1. 文章の要約

メールや、打ち合わせのメモ書きなどから、文章を要約してくれます。業務上のデータを扱う再には、プライバシー(個人名など)や、機密情報(公開できない情報)は、削除するか、別の文字に置き換えてください。

Prompt:
```cmd
### 指示 ###
以下の文章を140文字程度に要約をしてください。

文章: ###
<<要約前の文章>>
###
```

```cmd
### 指示 ###
以下の文章の要点をリストアップしてください。次のアクションプランがあれば、それもリストアップしてください。

文章: ###
<<要約前の文章>>
###
```

Promot:

```cmd
### 役割 ###
あなたは大学などの高等専門教育機関で、学生にLLMの教育をしているエキスパートです。

### 指示 ###
ChatGPTを使った Prompt を学ぶためのプランを作成してください。プランでは、要約、ロール定義、Few-Shot Learning、を取り上げてください。学習者がよくある間違いを示す例を幾つか考えてください。具体的な課題も作成してください。
```

## 1.2. 例示

答えてほしい書式や分類・相対的な数値(0-100点の間など)を「例」として示します。
この例の場合「すげぇ」は、実際に評価したい単語や文章を入力します。

Promopt:
```cmd
説明文は出力しないでください。

最高: Positive, 100 point
ダメじゃん: Negative, 5 point
すげぇ:
```

## 1.3. 添削

文章の中の機密情報・個人情報は、{A様}や{株式会社B社様}の様な、特定できない情報に置き換えてください。

謝罪メールの添削
Promot:
```cmd
以下の文章を内容は変更せずに、最大限考えうる謝罪のメールの文章にしてください。
何を添削したのかの解説を {改善点} にてリストアップして説明をしてください。

文章 ##
畠山さん。先日は飛行機の遅延があったとはいえ、15分も会議に遅れてすいませんでした。今後は気を付けます
###

```

文章は、ご自分で英作文をして置き換えてください😊

こちらの「1つ上のレベルの英文の作成」を実施してください。

[英文の添削](/教育/英文の採点.md)

## 1.4. 文章から表の作成

文章の中から、共通事項を見出だして、Excelのような表形式のデータを作成してくれます。

Prompt:
```cmd
### 指示 ###
構造化されていない文章が提供されます。それをCSV形式のデータを作成してください

文章: ###
最近発見された惑星グークラックスにはたくさんの果物がある。ネオスキズルは紫色でキャンディのような味がする。ロヘックルは灰色がかった青い果物で、レモンのような酸味がある。プーニッツは鮮やかな緑色で、甘いというより香ばしい。ネオンピンクで綿菓子のような味のループノバもたくさんある。最後に、酸味と苛性のある非常に酸っぱい苦味と、淡いオレンジ色を帯びたグロールと呼ばれる果物がある。
###
```


## 1.5. 簡単なプログラムの作成

以下のPromptを実行して、HTMLの文字列を作成します。その文字列をメモ帳などのテキストエディターにコピーして、「helloworld.html」というファイル名で、任意の場所に保存をします。そのファイルを任意のブラウザーで開いて、テキストボックスにご自身の名前を入力して、ボタンをおしてみてください。

Prompt:
```cmd
以下を実行する JavaSctipt のプログラムコードを作成してください。

Web画面構成:
Webの画面に以下が置かれています。
ラベル
テキストボックスボタン
ボタン

コード:
ボタンををクリックしたら、「ようこそ」という文字と、テキストボックスに入力された文字列を結合させて、メッセージボックスに表示します。

```


# 2. 実践

## 2.1. 調査結果からのレポート作成

以下は、Prompt ではありません。ご自身が仕事としてやる事として、Bing Chat や ChatGPT を使って実施してください。

課題:
ChatGPTの利用状況について調査をしてください。各国、各業種での具体的な利用事例を纏めます。企業が導入する上でのメリット・デメリットを挙げてください。

## 2.2. 会議のシュミレーション

「### 条件 ###」から先は、ご自身で今議論中のものに置き換えてください。
**{情報}** については、Bing Chat で以下のようなPromptを入力して情報を集めてください。

例:
```cmd
ChatGPTを企業が導入する上での、メリットとデメリットをリストアップしてください。
```


[会議のシュミレーション](/会議/ディスカッションをさせる.md)

思考方法については、「水平思考」以外も試してください。

思考の方向性を定義:

[思考の方向性](/HelloWorld%20-%20はじめの一歩.md)