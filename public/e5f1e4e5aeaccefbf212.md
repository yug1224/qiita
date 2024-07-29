---
title: NFCタグカードでデジタル名刺を自作しよう！
tags:
  - NFC
  - 名刺
  - QiitaEngineerFesta2024
private: false
updated_at: '2024-07-12T11:04:04+09:00'
id: e5f1e4e5aeaccefbf212
organization_url_name: hrbrain
slide: false
ignorePublish: false
---

## はじめに

こんにちは。[@yug1224（Yuji Yamaguchi）](https://x.com/yug1224)です。

勉強会やカンファレンスなどで「SNSアカウントをもっとスマートに共有したい！」と思う時ありますよね？

今回はNFCタグカードを使って自分で作るデジタル名刺をご紹介します！

![7e0054e8-dd48-c9f4-8341-a21d445792cd.gif](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/106236/7e0054e8-dd48-c9f4-8341-a21d445792cd.gif)

## NFCタグカードとは？

> NFCは、Near Field Communicationの略称で、13.56 MHzの周波数を利用する通信距離10cm程度の近距離無線通信技術です。非接触ICカードの通信および機器間相互通信が可能で、機器を近づけることで通信を行うため、「かざす」動作をきっかけにした、わかりやすい通信手段として注目を集めています。

[ソニー株式会社 | FeliCa | NFCについて | NFCの定義](https://www.sony.co.jp/Products/felica/NFC/#:~:text=NFC%E3%81%AF%E3%80%81Near%20Field%20Communication%E3%81%AE%E7%95%A5%E7%A7%B0%E3%81%A7%E3%80%8113.56%20MHz%E3%81%AE%E5%91%A8%E6%B3%A2%E6%95%B0%E3%82%92%E5%88%A9%E7%94%A8%E3%81%99%E3%82%8B%E9%80%9A%E4%BF%A1%E8%B7%9D%E9%9B%A210cm%E7%A8%8B%E5%BA%A6%E3%81%AE%E8%BF%91%E8%B7%9D%E9%9B%A2%E7%84%A1%E7%B7%9A%E9%80%9A%E4%BF%A1%E6%8A%80%E8%A1%93%E3%81%A7%E3%81%99%E3%80%82%E9%9D%9E%E6%8E%A5%E8%A7%A6IC%E3%82%AB%E3%83%BC%E3%83%89%E3%81%AE%E9%80%9A%E4%BF%A1%E3%81%8A%E3%82%88%E3%81%B3%E6%A9%9F%E5%99%A8%E9%96%93%E7%9B%B8%E4%BA%92%E9%80%9A%E4%BF%A1%E3%81%8C%E5%8F%AF%E8%83%BD%E3%81%A7%E3%80%81%E6%A9%9F%E5%99%A8%E3%82%92%E8%BF%91%E3%81%A5%E3%81%91%E3%82%8B%E3%81%93%E3%81%A8%E3%81%A7%E9%80%9A%E4%BF%A1%E3%82%92%E8%A1%8C%E3%81%86%E3%81%9F%E3%82%81%E3%80%81%E3%80%8C%E3%81%8B%E3%81%96%E3%81%99%E3%80%8D%E5%8B%95%E4%BD%9C%E3%82%92%E3%81%8D%E3%81%A3%E3%81%8B%E3%81%91%E3%81%AB%E3%81%97%E3%81%9F%E3%80%81%E3%82%8F%E3%81%8B%E3%82%8A%E3%82%84%E3%81%99%E3%81%84%E9%80%9A%E4%BF%A1%E6%89%8B%E6%AE%B5%E3%81%A8%E3%81%97%E3%81%A6%E6%B3%A8%E7%9B%AE%E3%82%92%E9%9B%86%E3%82%81%E3%81%A6%E3%81%84%E3%81%BE%E3%81%99%E3%80%82)

NFCタグカードとは、NFC技術を使ってデータの読み書きができるカードです。

スマートフォンをかざすだけで、あらかじめ登録しておいた情報を読み取ることができます。

## 必要なもの

- NFCタグ
- NFC対応のスマートフォン
- プロフィールページ

必要なものは上記のみ。ICカードリーダーライターなどは不要です。

NFCタグはAmazonで検索するといろいろな形のものが出てくるので、好きなものを選んでください。

今回は、「デジタル名刺」なのでカード型を選択します。

https://www.amazon.co.jp/dp/B0CGMH2QZ6

## 手順 1. プロフィールページを作ろう！

NFCを読み取った際にアクセスさせるためのURLを用意します。

XやGitHubのプロフィールページでも良いですが、複数の情報を共有できるプロフィール作成サービスを利用するのもオススメです！

今回は、リッチでキレイなプロフィールページを作成できる「[Bento](https://bento.me/)」を利用します。

https://bento.me/yug1224

## 手順 2. NFCタグにURLを書き込もう！

Apple App Store

https://apps.apple.com/jp/app/nfc-tools/id1252962749

Google Play ストア

https://play.google.com/store/apps/details?id=com.wakdev.wdnfc

NFCタグに情報を書き込むために、まずはNFC対応のスマートフォンに「NFC Tools」というアプリをインストールしてください。

![ef4370f7-f39e-d2dc-8007-b0b5bd114ec2.gif](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/106236/ef4370f7-f39e-d2dc-8007-b0b5bd114ec2.gif)

アプリを起動し、「書く」「レコードを追加」「URL/URI」と進み、URLを入力し「OK」。

「書き込み」を押下すると、スキャン待機状態になるのでカードをかざしてください。

「✓」が表示されたら書き込み完了です。

## 手順 3. NFCタグに書き込んだURLを読み取ってみよう！

![de06f779-d02f-21d8-c0e9-010fc2081a86.gif](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/106236/de06f779-d02f-21d8-c0e9-010fc2081a86.gif)

NFCをスマートフォンにかざすと、スマートフォンが情報を読み取ってくれます。

iPhoneの場合は通知バーが表示されるので、これを押下するとSafariが起動し、ページが表示されます。

## まとめ

![fb3f5b40-8801-e02a-de32-7a0f017b197a.jpeg](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/106236/fb3f5b40-8801-e02a-de32-7a0f017b197a.jpeg)

NFCタグカードを使ってデジタル名刺を自作する方法を紹介しました！

簡単に作成できるので、ぜひ試してみてください！

自分はさらに[ラクスル](https://raksul.com/)で作ったステッカーを貼ったりしています。

## PR

HRBrainでは一緒に働く仲間を募集しています。歴史に残るトライをしよう！

https://www.hrbrain.co.jp/recruit
