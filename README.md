[![CI](https://github.com/rao-donut/tribal-hunter-translate-ja/actions/workflows/checkJSON.yml/badge.svg?branch=main)](https://github.com/rao-donut/tribal-hunter-translate-ja/actions/workflows/checkJSON.yml)

# tribal-hunter-translate-ja

Tribal Hunterの日本語訳公式リポジトリです。
翻訳のご協力をよろしくお願いいたします！

専用のDiscordサーバを立てています。ぜひご参加ください。
https://discord.gg/GP6PnqqeEb

## 作業の進め方

ゲームをプレイしたあとに翻訳するのがおすすめです。
ゲームは次のURLからダウンロードできます！

[Steam - Tribal Hunter](https://store.steampowered.com/app/1379870/Tribal_Hunter/)

また、作業をする際に困った点などがございましたら[こちら](https://twitter.com/RIORAO)のDMにご連絡ください。

### 0. 共通項目 - 翻訳されていないファイルを探す

[こちら](https://github.com/rao-donut/tribal-hunter-translate-ja/issues)から課題の一覧を確認できます。
作業がコンフリクトしないようにするため、翻訳するファイルが明確に決まりましたら、各Issueにコメントをしてください。
進行中のタスクは「**Processing**」ラベルがついています。

### 1. Gitが分かる人向け

#### 1-1. ブランチ作成

`main` ブランチから `username/xxxxxx` のようなブランチを切って作業をはじめます。 `xxxxxx` には、変更箇所や修正箇所などのトピックを記述してください。

#### 1-2. 翻訳者情報ファイルの記述

`contributor` ディレクトリに `username.txt` のファイルを作成し、以下のテンプレートに沿って署名してください。

署名された名前はゲームのクレジットに掲載させていただきます。

```
Name: username
```

#### 1-3. 翻訳作業

`ja` ディレクトリのファイルを開き、原文を翻訳して作業を進めてください。

#### 1-4. Pull Requests作成

`main` ブランチに向けたPull Requestsを作成してください。Pull Requestsの文言は、以下のテンプレートを使うと便利です。また、作業ブランチは必要に応じて `rebase -i` か `merge -squash` をしてください。

レビュアーには `rao-donut` を選択してください。

```
## 概要
<!-- どのような内容のPull Requestsなのかを記述 -->

## 確認項目
<!-- レビュアーに確認してほしい項目 -->

## 補足
<!-- 翻訳をした際に留意した点などを記述 -->
```

### 2. Gitがわからない人向け

#### 2-1. ファイルのダウンロード

「Code」と書かれた緑色のボタンをクリックし、「Download ZIP」を選択して現状のマスターファイルをダウンロードします。
ファイルは逐次更新されますので定期的に新しいマスターファイルをダウンロードしてください。

#### 2-2. 翻訳を行う

ファイルは `JSON` というフォーマットで記述されており、そのフォーマットにしたがってデータを作成する必要があります。

`"key": "value"` といったような形式で記述されます。編集する箇所は `"value"` の箇所です。 `"key"` は変更しないでください。

次に例を示します。

```
"room_Village": "Village"
```

この場合は `"Village"` を翻訳します。「Village」は「村」と訳せるので、編集後のデータは次のようになります。

```
"room_Village": "村"
```

#### 2-3. ファイルを送る

[@RIORAO](https://twitter.com/RIORAO)のDMかDiscord[ RAO(らお)#5959 ]に翻訳後のファイルをお送りください。

#### 2-4. ファイルが採用されたときは

翻訳協力者としてクレジットに掲載するために、掲載するニックネームを教えてください。
