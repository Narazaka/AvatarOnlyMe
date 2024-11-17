# OnlyMe and OnlyYouAndMe for Avatars

## インストール

### VCCによる方法

1. https://vpm.narazaka.net/ から「Add to VCC」ボタンを押してリポジトリをVCCにインストールします。
2. VCCでSettings→Packages→Installed Repositoriesの一覧中で「Narazaka VPM Listing」にチェックが付いていることを確認します。
3. アバタープロジェクトの「Manage Project」から「OnlyMe and OnlyYouAndMe for Avatars」をインストールします。

## OnlyMe

自分にだけしか見えないようにするやつ

1. OnlyMeプレハブをアバター内に置く
2. OnlyMeプレハブルートのMA Merge Animatorの「相対的パスのルート」に自分だけに表示したいオブジェクトを指定する
3. 自分だけに表示したいオブジェクトを非表示にする（GameObjectのチェックを外す）
    - これをやらないとセーフティでブロックされる相手に表示されてしまう

- 複数のオブジェクトでやりたい場合
  - 単純にその数分同様の手順で増やして下さい

## OnlyYouAndMe

自分とキー文字列を共有した人Aさんにだけしか見えないようにするやつ
1. OnlyYouAndMeプレハブをアバター内に置く
2. OnlyYouAndMeプレハブルートのMA Merge Animatorの「相対的パスのルート」に自分とAさんだけに表示したいオブジェクトを指定する
3. 自分とAさんだけに表示したいオブジェクトを非表示にする（GameObjectのチェックを外す）
    - これをやらないとセーフティでブロックされる相手に表示されてしまう
4. OnlyYouAndMe/Contacts/Containerの下にあるSenderとReceiver両方のCollision Tagsというところの文字列を他人に推測されないものにし、Aさんにも同じ値で同手順で導入してもらう。

- 複数のオブジェクトでやりたい場合
  - OnlyYouAndMeプレハブ直下にOnlyYouAndMeBaseを置いて、そちらの「相対的パスのルート」に追加のオブジェクトを指定して下さい。

## LICENSE

[Zlib License](LICENSE.txt)
