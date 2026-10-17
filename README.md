# PrisonAsset

刑務所マップ（[Prison](https://github.com/Avuorina/Prison)）用のリソースパック。対象は Minecraft Java Edition 26.3。

## 使い方
- **サーバーで配る**：[リリース](https://github.com/Avuorina/PrisonAsset/releases) の説明にある3行を `server.properties` に書く
- **自分で入れる**：リリースの `PrisonAsset.zip` を `resourcepacks` フォルダに入れる

## リリースの出し方
GitHub Actions が zip を作ってリリースに置く(SHA-1 も出す)。
- **main に push**(パックの中身が変わったとき)：リリース `latest` を作り直す。URL は変わらない
  `https://github.com/Avuorina/PrisonAsset/releases/download/latest/PrisonAsset.zip`
- **`v1` `v2` … のタグを push**：そのタグの固定版リリースを作る

SHA-1 は中身が変わるたびに変わるので、`server.properties` の `resource-pack-sha1` も書き直す。

## 見た目を切り替えているアイテム
`custom_model_data` の `strings` の1つ目で切り替える。

| アイテム | strings | モデル |
| --- | --- | --- |
| trial_key | key_light_blue / key_blue / key_red / key_yellow / key_purple | prison:item/key_* |
| ominous_trial_key | key_master | prison:item/key_master |
| stick | baton | prison:item/baton |
| lead | handcuffs | prison:item/handcuffs |
| carrot_on_a_stick | camera_remote / schedule_speed | 表示しない(minecraft:empty) |

## 元データ
Blockbench の `.bbmodel` は `blockbench/` に置く。

## item_model で直接使うもの
`item_model` コンポーネントで指定する。

| item_model | 使う場面 |
| --- | --- |
| prison:camera | 監視カメラの模型(item_display) |
