## woolisbest youtube
# youtubeについて
利用するときはlssuesで言ってください（リポジトリのリンクもお願いします。）
### youtubeeducationのパラメーターです。
２日に一回ほど更新します。
```
https://youtubeeducation.com/embed/{videoID}{parameter}
```
のような形式で使ってください。
# パラメーターの形式を変更しました。　確認してください。
サイトに組み込む場合は
[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/parameter.txt)か
[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/edu.txt)です。

新しいものを追加しました。
[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/ep.txt)

他の方が更新しているものです。

[幸せok](https://raw.githubusercontent.com/siawaseok3/wakame/master/video_config.json)

[わかめ](https://raw.githubusercontent.com/wakame02/wktopu/refs/heads/main/edu.text)

[Toka_Kun_1](https://raw.githubusercontent.com/toka-kun/Education/refs/heads/main/keys/key1.json)

[Toka_Kun_2](https://raw.githubusercontent.com/toka-kun/Education/refs/heads/main/keys/key2.json)

[hgkf01001_1](https://raw.githubusercontent.com/70142-lgtm/hgkf-Tube/refs/heads/main/hgkf01001_1.txt)

[hgkf01001_2](https://raw.githubusercontent.com/70142-lgtm/hgkf-Tube/refs/heads/main/hgkf01001_2.txt)
## ストリーム再生などのAPIです。
### invidious
現在（11/15)使用可能なものです。

javascriptで読み込めるように.jsonファイルにしてあります。 [こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/inv.json)

現在(11/15)使用できないものです。
使えないものなので.txt形式です。　[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/inv-no.txt)

### pipedAPI
pipedのAPIです。[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/piped.txt)

### 動画ダウンロード用のAPI（？）などです。
[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/downloadAPI.txt)
### ストリーム再生の取得用URLです。
間違っていたらすいません。

[こちら](https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/stream.txt)

# YouTube 埋め込みパラメータ一覧（2025 最新）

---

## 🎛 基本再生コントロール

| パラメータ | 値の例 | 説明 | 現行ステータス |
|------------|--------|-------|----------------|
| `autoplay` | 0 / 1 | 自動再生（※ミュート必須） | ✔ 有効 |
| `mute` | 0 / 1 | ミュート再生 | ✔ 有効 |
| `controls` | 0 / 1 | コントロールバー表示（0 は一部無効） | ✔ 有効 |
| `loop` | 0 / 1 | ループ再生 | ✔ 有効（`playlist` 必須） |
| `playlist` | VIDEO_ID | ループ元 / プレイリスト | ✔ 有効 |
| `start` | 秒数 | 再生開始位置 | ✔ 有効 |
| `end` | 秒数 | 再生終了位置 | ✔ 有効 |
| `playsinline` | 0 / 1 | スマホでインライン再生 | ✔ 有効 |
| `enablejsapi` | 1 | IFrame API 使用許可 | ✔ 有効 |

---

## 🎨 表示設定

| パラメータ | 値の例 | 説明 | 現行ステータス |
|------------|--------|-------|----------------|
| `modestbranding` | 1 | YouTube ロゴを最小化 | ✔ 有効 |
| `rel` | 0 / 1 | 関連動画（0 でも同チャンネル動画は表示） | ▣ 仕様変更により部分有効 |
| `iv_load_policy` | 1 / 3 | 注釈（Info カード）表示設定 | ✔ 有効 |
| `cc_load_policy` | 1 | 字幕を強制オン | ✔ 有効 |
| `color` | red / white | プレイヤー UI の色 | ▣ 一部のみ有効 |

---

## 🧰 再生制限・操作制御

| パラメータ | 値の例 | 説明 | 現行ステータス |
|------------|--------|-------|----------------|
| `fs` | 0 / 1 | 全画面ボタンの有無 | ✔ 有効 |
| `disablekb` | 0 / 1 | キーボード操作を無効化 | ✔ 有効 |

---

## ❌ 廃止 / 無効化されたパラメータ

| パラメータ | 説明 |
|------------|------|
| `showinfo` | タイトル非表示（廃止） |
| `autohide` | コントロール自動非表示（廃止） |
| `theme` | dark / light テーマ（廃止） |
| `version` | Flash 時代のパラメータ |
| `rel=0`（完全非表示） | 現在は完全オフ不可能 |
| `origin` | IFrame API 使用時は自動付与のため不要 |

---

## 📦 すべてのパラメータ入り iframe サンプル

<details>
<summary>クリックして展開</summary>

```html
<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/VIDEO_ID?
    autoplay=1&
    mute=1&
    controls=1&
    loop=1&
    playlist=VIDEO_ID&
    start=10&
    end=60&
    playsinline=1&
    modestbranding=1&
    rel=0&
    cc_load_policy=1&
    iv_load_policy=3&
    fs=1&
    disablekb=0&
    enablejsapi=1"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen
></iframe>
