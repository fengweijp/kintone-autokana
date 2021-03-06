# kintone漢字かな変換プラグイン 

## 概要

* 入力フォームで、あらかじめ指定した「漢字フイールド」に日本語を入力すると、自動的に「かなフィールド」にふりがなが入ります。

* 内部で [jQuery.autoKana](https://github.com/harisenbon/autokana "autokana") プラグインを使用しています。

## 使い方

* release/kintone-autokana_vXX.zipをkintoneの管理画面よりプラグインとして追加します。

* 適用するアプリの 詳細設定−プラグイン より、「漢字かな変換プラグイン」を有効にします。

* 漢字かな変換プラグインの設定画面で「漢字フィールド」「かなフィールド」を指定します。
  * （例）漢字フィールド：担当者名  かなフィールド：担当者名かな
  * 漢字フィールド、かなフィールドはあらかじめフォームに追加しておく必要があります。

## 注意

現バージョン（version 1）では以下の制約があります。

* 漢字・かなフィールドに指定できるのは1組だけです。

* ひらがなへの変換のみ対応しています。カタカナへの変換はできません。
  * jQuery.autoKana はカタカナにも対応していますので、次期バージョンで機能追加の予定です。
