# AV ゼウス

あなたの好みの AV を AI がオススメしてくれる Web アプリです。

## お知らせ

※現在開発中です。

## 各サービスの GitHub リポジトリ

- **AI Engine**：[Kan0620/avzeus-recommend_AI](https://github.com/Kan0620/avzeus-recommend_AI)
- **Backend**：[souhub/avzeus-backend](https://github.com/souhub/avzeus-backend)
- **Frontend**：[souhub/avzeus-frontend](https://github.com/souhub/avzeus-frontend)

## 使い方

1. トップページ
   トップページです。ボタンを押して始めます。
   ![トップページ](assets/top.png)

2. 説明ページ
   説明ページです。使い方の説明を簡単に行います。
   ![説明ページ](assets/explanation.png)

3. 選択ページ
   ![選択ページ](assets/selection)
   表示された女性の写真の中から好みの人を 5 人選択します。

4. 結果ページ
   ![結果ページ](assets/recommendation)
   AI が選択された情報を元にあなた好みのオススメ AV を表示します。<br/>
   AI は確率考慮と強化学習を行うため、同じ結果を入力しても結果が異なる場合もあります。

## 使用技術

使った主な技術は以下のとおりです。

- Docker v20.10.5
- Docker Compose v1.28.5
- Docker Hub
- Go v1.15
- Python v3.9.0
- Flask v1.1.2
- JavaScript
- Vue.js v3
- CSS
- MySQL v8.0.23
- Google Cloud Storage
- Google Kubernetes Engine
- DMM API
- [moqups](https://moqups.com/)

## 環境

開発環境と本番環境はそれぞれ以下の図の通りです。
<br/><br/>
**【開発環境】**<br/>
Docker でマイクロサービス化させ、Docker Compose で連携させています。<br/><br/>
**【本番環境】**<br/>
Docker でマイクロサービス化させ、Google Kubernetes Engine で連携させています。<br/>
データベースは開発環境とは異なり、Docker 化せずに、Cloud SQL を使用しています。<br/><br/>
![環境図](assets/envs.png)
