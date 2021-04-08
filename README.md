# AV ゼウス

あなたの好みの AV を AI がオススメしてくれる Web アプリです。

## お知らせ

~~※現在開発中です。~~ <br/>
2021/4/8 追記<br/>
β 版をリリースしました。<br/>

https://avzeus-client.mmu6fa6rgrojg.ap-northeast-1.cs.amazonlightsail.com/

## 各サービスの GitHub リポジトリ

- **AI Engine**：[Kan0620/avzeus-recommend_AI](https://github.com/Kan0620/avzeus-recommend_AI)
- **Backend**：[souhub/avzeus-backend](https://github.com/souhub/avzeus-backend)
- **Frontend**：[souhub/avzeus-frontend](https://github.com/souhub/avzeus-frontend)

## 使い方

1. トップページ<br/><br/>
   トップページです。ボタンを押して始めます。<br/><br/>
   ![トップページ](assets/top.png)<br/>

2. 説明ページ<br/><br/>
   説明ページです。使い方の説明を簡単に行います。<br/><br/>
   ![説明ページ](assets/explanation.png)<br/>

3. 選択ページ<br/><br/>
   表示された女性の写真の中から好みの人を 5 人選択します。<br/><br/>
   ![選択ページ](assets/selection.png)<br/>

4. 結果ページ<br/><br/>
   AI が選択された情報を元にあなた好みのオススメ AV を表示します。<br/>
   AI は確率考慮と強化学習を行うため、同じ結果を入力しても結果が異なる場合もあります。<br/><br/>
   ![結果ページ](assets/recommendation.png)<br/>

## 使用技術

使った主な技術は以下のとおりです。<br/><br/>
![用いた技術](assets/technologies.png)

- Docker v20.10.5
- Docker Compose v1.28.5
- Go v1.15
- Python v3.9.0
- JavaScript
- Flask v1.1.2
- Vue.js v3
- Nginx
- MySQL v8.0.23
- Google Cloud Storage
- Amazon Lightsail
- CircleCI
- moqups
- draw.io

## 環境

開発環境と本番環境はそれぞれ以下の図の通りです。
<br/><br/>
**【開発環境】**<br/>
Docker で下図のように 4 つのサーバーに分け、Docker Compose で連携させています。<br/><br/>
**【本番環境】**<br/>
下図のように 3 つのサーバーにわけています。<br/>
データベースは開発環境とは異なり、Docker 化せずに、Loghtsail データベース を使用しています。<br/><br/>
![環境図](assets/envs.png)
