## ゲームのとも（Game Progress Buddy API）

### 概要

- ゲームを途中までで止めがち、どこまでやったか分かんなくなってしまうおれ用のアプリ

### 作るもの

- 画面
- ゲーム情報取得API　{host}/api/game-select  [GET]
- ゲームマスタ登録API　{host}/api/game-insert  [POST]
- ゲーム記録登録API　{host}/api/game-detail-insert  [POST]
- ゲーム記録更新API　{host}/api/game-detail-update [PUT]
- ゲーム記録削除API　{host}/api/game-detail-delete [DELETE]
- ゲームマスタ削除API 　{host}/api/game-delete [DELETE]
- ゲームマスタ　GAME_MST
- ゲームマスタ　GAME_DETAIL_TRN

### テーブル

#### ゲームマスタ
- ゲームID
- ゲーム名
- 登録日
- クリア済フラグ
- プレイ済フラグ
- 削除フラグ
  
#### ゲーム記録トラン
- ゲームID
- ゲーム名
- 最終プレイ日
- 最終プレイ記録
- 次やること
