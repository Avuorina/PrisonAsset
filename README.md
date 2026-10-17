# PrisonAsset

刑務所マップ（[Prison](https://github.com/Avuorina/Prison)）用のリソースパック。対象は Minecraft Java Edition 26.3。

## 使い方
このリポジトリの中身（`pack.mcmeta` と `assets/`）を zip にして `resourcepacks` フォルダに入れる。

## 見た目を切り替えているアイテム
`custom_model_data` の `strings` の1つ目で切り替える。

| アイテム | strings | モデル |
| --- | --- | --- |
| trial_key | key_light_blue / key_blue / key_red / key_yellow / key_purple | prison:item/key_* |
| ominous_trial_key | key_master | prison:item/key_master |
| stick | baton | prison:item/baton |
| lead | handcuffs | prison:item/handcuffs |

## 元データ
Blockbench の `.bbmodel` は `blockbench/` に置く。
