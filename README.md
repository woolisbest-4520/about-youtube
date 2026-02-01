about-youtube / youtubeeducation
================================

YouTube 埋め込み・ストリーム再生・代替 API 情報まとめ
youtubeeducation を中心としたパラメータ・API 管理用テキスト

--------------------------------
【利用上の注意】
--------------------------------
・利用時は必ず Issues で連絡してください
・使用先のリポジトリ URL を明記してください
・パラメータ / API は頻繁に更新されます（目安：2日に1回）

--------------------------------
【youtubeeducation 埋め込み形式】
--------------------------------
https://youtubeeducation.com/embed/{videoID}{parameter}

例：
https://youtubeeducation.com/embed/VIDEO_ID?autoplay=1&mute=1

--------------------------------
【youtubeeducation パラメータ定義】
--------------------------------

▼ parameter.txt
GitHub Raw:
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/parameter.txt

jsDelivr:
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/parameter.txt

GitHack:
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/parameter.txt


▼ edu.txt
GitHub Raw:
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/edu.txt

jsDelivr:
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/edu.txt

GitHack:
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/edu.txt


▼ ep.txt（新規追加）
GitHub Raw:
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/ep.txt

jsDelivr:
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/ep.txt

GitHack:
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/ep.txt

--------------------------------
【他ユーザー管理（本リポジトリ外）】
--------------------------------

▼ 幸せok
https://raw.githubusercontent.com/siawaseok3/wakame/master/video_config.json

▼ わかめ
https://raw.githubusercontent.com/wakame02/wktopu/refs/heads/main/edu.text

▼ Toka_Kun
https://raw.githubusercontent.com/toka-kun/Education/refs/heads/main/keys/key1.json
https://raw.githubusercontent.com/toka-kun/Education/refs/heads/main/keys/key2.json

▼ hgkf01001
https://raw.githubusercontent.com/70142-lgtm/hgkf-Tube/refs/heads/main/hgkf01001_1.txt
https://raw.githubusercontent.com/70142-lgtm/hgkf-Tube/refs/heads/main/hgkf01001_2.txt

--------------------------------
【ストリーム再生 / API】
--------------------------------

▼ Invidious（使用可能：11/15 時点）
GitHub Raw:
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/inv.json

jsDelivr:
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/stream/inv.json

GitHack:
https://raw.githack.com/woolisbest-4520/about-youtube/main/stream/inv.json


▼ Invidious（使用不可）
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/inv-no.txt


▼ Piped API
GitHub Raw:
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/piped.txt

jsDelivr:
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/stream/piped.txt

GitHack:
https://raw.githack.com/woolisbest-4520/about-youtube/main/stream/piped.txt


▼ 動画ダウンロード用 API（参考）
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/downloadAPI.txt


▼ ストリーム取得 URL（参考・未検証）
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/stream.txt

--------------------------------
【YouTube 埋め込みパラメータ（2025）】
--------------------------------

有効：
autoplay (mute 必須)
mute
controls
loop（playlist 必須）
playlist
start / end
playsinline
enablejsapi
modestbranding
iv_load_policy
cc_load_policy
fs
disablekb

部分有効：
rel
color

廃止・無効：
showinfo
autohide
theme
version
完全な rel=0
origin

--------------------------------
【注意】
--------------------------------
・jsDelivr はキャッシュされます（即時反映されない場合あり）
・GitHack は表示・埋め込み用途向け
・最新性が必要な場合は GitHub Raw を推奨
