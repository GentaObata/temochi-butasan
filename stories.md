# 実装したいこと

## リリースまでに最低限必要なこと
- [x] 画像の画質を高くする
- [x] 文字の色を合わせる
- [x] クリアの時間を表示する
- [x] 開いた時のstatusで表示が変わる
- [x] finish時のダイアログの中身
- [ ] 計測ツールの実装？　確認を先に
- [ ] アイコン
- [ ] その他申請に必要な物の準備

## 基本機能
- [x] nodeを継承した豚クラスを作る
  -x[ ] 豚は速度を持つ
- [x] スワイプした方向に一定速度で豚が移動する
  - [x] 豚の速度にそって豚は動き続ける
  - [x] スワイプしてから離すと豚に一定の速度を与える
- [x] 跳ね返るごとに豚の速度が減衰する
- [x] 画面端で豚が跳ね返る
  - [x] 跳ね返る時に触覚FBを起こす
- [x] スワイプをはなした時の勢いに応じて豚の初速を変える
- [x] 掴んだら速度と回転を止める
- [x] スワイプして豚を画面端に持っていても豚がはみ出さない（枠を太くすれば解決する？？）
- [x] ドラッグで壁に寄せた時にFBが発生しないように（速度の制限をつければOKそう　あるいはタップ中は反応しないとか 両方必要か）
- [ ] スワイプへの反応をもっと自然にする
- [ ] 画面外にもってこうとするとびよんってなるやつの解消。はみ出さなくしても、結局起きている
- [ ] 指でスワイプしてはみ出してしまうことの解決のブラッシュアップ
- [ ] 指と豚の位置関係を保持する
- [ ] 速度によってFBの大きさが変わる
- [ ] 進むごとに豚が減衰する。摩擦ではない説
- [ ] 画像の画質を高くする
- [ ] 文字の色を合わせる
- [ ] チュートリアルを豚の下にする
- [x] クリアの時間を表示する
- [ ] fontをいい感じのものにする。全体で合わせる
- [ ] buttonタップ時の色とかで押した感だす

## 発展的なアイデア
- [ ] 端末の重力加速度で重力を与える
- [ ] ブタを二匹にする
- [ ] 障害物を設置する
- [ ] 掴んだ位置をもとに力を加える
- [ ] 命令的すぎるからRxを使って宣言的に書き直したい

## ゲーム要素
- [x] 目標点数機能
  - [x] 目標点数の回数だけ豚を跳ね返らせることを目指す
    - [x] labelの表示
    - [x] stageの実装
      - [x] 目標値の設定
      - [x] 現在のカウントの保持
      - [x] 衝突イベントを元にカウントの増減
      - [x] クリア時のイベント？　　
    - [x] stage model
      - [x] stageをもつ
      - [x] ゲームの起動とともにstageを呼び出す
      - [x] gameSceneのイベントをもとにstageを書き換え
      - [x] データの保存はstageを保存するかたち
      - [x] game SceneをviewControllerとみたてる
        - [x] stageの変更をdelegateでSceneに伝える
        - [x] Sceneはそれを元に、labelを書き換える
  - [ ] あたりかたで点数の減り方が変わる
  - [x] 開いた時のstatusで表示が変わる
  - [x] finish時のダイアログの中身
  - [x] クリアすると次の目標が与られる
    - [ ] 豚の種類や、背景などをアンロックできる
  - [x] 目標はその都度高くなる
  - [x] 今のレベルと点数を端末内部に保存する
- [ ] 豚の種類によって点数の減り方がかわる
- [ ] ゲーム中のポイントや課金で豚を買える
- [ ] 背景を変えられる機能
  - [ ] 宇宙で無重力感だすとか
- [ ] ログイン機能
  - [ ] データを保存できる
- [ ] ステージにもっとこだわる
  - [ ] ステージごとに背景が違う
  - [ ] ステージごとにメッセージが違う
  - [ ] ポイントの設定が単調ではない


## 開発環境
- [ ] ビルドスキームを整える
  - [ ] develop
  - [ ] release
- [x] app stpreへの申請する準備
- [x] UITest環境を用意する
- [ ] UnitTest環境を用意する
