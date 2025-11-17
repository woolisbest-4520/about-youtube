## woolisbest youtube
# youtubeについて
### youtubeeducationのパラメーターです。
２日に一回ほど更新します。
```
https://youtubeeducation.com/embed/{videoID}{parameter}
```
のような形式で使ってください。
サイトに組み込む場合は[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/parameter.json)か
[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu.json)です。
他の方が更新しているものです。

[幸せok](https://raw.githubusercontent.com/siawaseok3/wakame/master/video_config.json)

[わかめ](https://raw.githubusercontent.com/wakame02/wktopu/refs/heads/main/edu.text)
## ストリーム再生などのAPIです。
### invidious
現在（11/15)使用可能なものです。

javascriptで読み込めるように.jsonファイルにしてあります。 [こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/inv.json)

現在(11/15)使用できないものです。
使えないものなので.txt形式です。　[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/inv-no.txt)

### pipedAPI
pipedのAPIです。[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/piped.txt)

### 動画ダウンロード用のAPI（？）などです。
[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/downloadAPI.txt)
### ストリーム再生の取得用URLです。
間違っていたらすいません。

[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream.txt)

## youtube埋め込みのパラメーター解説
### 基本再生制御
```
|パラメータ 　 |値の例   |	説明|	現行ステータス
|autoplay    	|0 / 1   |	自動再生（※ミュートが必須）	有効
|mute	        |0 / 1   | ミュート再生	有効
|controls	    |0 / 1   | コントロールバー表示（0 は制限あり）	有効
|loop	        |0 / 1   |	ループ再生	有効（playlist 必須）
|playlist    	|VIDEO_ID|	loop 用 or 複数動画	有効
|start	      |秒数    |	開始位置	有効
|end	        |秒数    | 終了位置	有効
|playsinline	|0 / 1   |	スマホでインライン再生	有効
|enablejsapi	|1	     | IFrame API 使用	有効
```
### 表示設定
```
パラメータ	値の例	説明	現行ステータス
modestbranding	1	YouTube ロゴを最小化	有効
rel	0 / 1	関連動画（0でも同一チャンネルは出る）	仕様変更済だが動作
iv_load_policy	1 / 3	動画の注釈（カード）表示設定	有効
cc_load_policy	1	字幕を強制オン	有効
color	red / white	コントロール色	一部のみ有効
```
### 制限 / 操作制御
```
パラメータ	値の例	説明	現行ステータス
fs	0 / 1	全画面ボタン制御	有効
disablekb	0 / 1	キーボード操作を無効化	有効
```
### 現在は無効 / 非推奨パラメータ
```
パラメータ	説明
showinfo	再生前のタイトル非表示（廃止）
autohide	コントロールバー自動隠し（廃止）
theme	dark / light のテーマ（廃止）
version	古い Flash 系（廃止）
rel=0（完全非表示）	現在は同チャンネル動画が表示される
origin	IFrame API では自動付与になった
```
