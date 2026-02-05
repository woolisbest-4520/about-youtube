# about-youtube / youtubeeducation
YouTube 埋め込み・ストリーム再生・代替 API 情報まとめ  
youtubeeducation を中心としたパラメータ・API 管理用ドキュメント

---

# 目次
1. 利用上の注意  
2. youtubeeducation 埋め込み形式  
3. パラメータ定義ファイル  
4. 他ユーザー管理（外部リポジトリ）  
5. ストリーム再生 / API  
6. YouTube 埋め込みパラメータ（2025）  
7. パラメータ一覧（表形式）  
8. 注意  
9. README（英語版）  
10. README（スペイン語版）  
11. README（オランダ語版）  
12. README（中国語版）  
13. README（韓国語版）  
14. README（フランス語版）  
15. README（ドイツ語版）

---

## 1. 利用上の注意
- 利用時は必ず Issues で連絡してください  
- 使用先のリポジトリ URL を明記してください  
- パラメータ / API は頻繁に更新されます（目安：2日に1回）

---

## 2. youtubeeducation 埋め込み形式

埋め込み URL 形式：  
`https://youtubeeducation.com/embed/{videoID}{parameter}`

例：  
`https://youtubeeducation.com/embed/VIDEO_ID?autoplay=1&mute=1`

---

## 3. パラメータ定義ファイル

### parameter.txt
GitHub Raw:  
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/parameter.txt  
jsDelivr:  
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/parameter.txt  
GitHack:  
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/parameter.txt  

### edu.txt
GitHub Raw:  
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/edu.txt  
jsDelivr:  
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/edu.txt  
GitHack:  
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/edu.txt  

### ep.txt
GitHub Raw:  
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/ep.txt  
jsDelivr:  
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/ep.txt  
GitHack:  
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/ep.txt  

### key1.txt
GitHub Raw:  
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/key1.txt  
jsDelivr:  
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/key1.txt  
GitHack:  
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/key1.txt  

### key2.txt
GitHub Raw:  
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/edu/key2.txt  
jsDelivr:  
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/edu/key2.txt  
GitHack:  
https://raw.githack.com/woolisbest-4520/about-youtube/main/edu/key2.txt  

---

## 4. 他ユーザー管理（外部リポジトリ）

幸せok  
https://raw.githubusercontent.com/siawaseok3/wakame/master/video_config.json

わかめ  
https://raw.githubusercontent.com/wakame02/wktopu/refs/heads/main/edu.text

Toka_Kun  
https://raw.githubusercontent.com/toka-kun/Education/refs/heads/main/keys/key1.json  
https://raw.githubusercontent.com/toka-kun/Education/refs/heads/main/keys/key2.json

hgkf01001  
https://raw.githubusercontent.com/70142-lgtm/hgkf-Tube/refs/heads/main/hgkf01001_1.txt  
https://raw.githubusercontent.com/70142-lgtm/hgkf-Tube/refs/heads/main/hgkf01001_2.txt

---

## 5. ストリーム再生 / API

### Invidious（使用可能）
GitHub Raw:  
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/inv.json  
jsDelivr:  
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/stream/inv.json  
GitHack:  
https://raw.githack.com/woolisbest-4520/about-youtube/main/stream/inv.json  

### Invidious（使用不可）
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/inv-no.txt

### Piped API
GitHub Raw:  
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/piped.txt  
jsDelivr:  
https://cdn.jsdelivr.net/gh/woolisbest-4520/about-youtube@main/stream/piped.txt  
GitHack:  
https://raw.githack.com/woolisbest-4520/about-youtube/main/stream/piped.txt  

### 動画ダウンロード用 API（参考）
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/downloadAPI.txt

### ストリーム取得 URL（参考・未検証）
https://raw.githubusercontent.com/woolisbest-4520/about-youtube/refs/heads/main/stream/stream.txt

---

## 6. YouTube 埋め込みパラメータ（2025）

### 有効
autoplay（mute 必須）  
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

### 部分有効
rel  
color  

### 廃止・無効
showinfo  
autohide  
theme  
version  
完全な rel=0  
origin  

---

## 7. パラメータ一覧（表形式）

| パラメータ | 状態 | 備考 |
|-----------|------|------|
| autoplay | 有効 | mute 必須 |
| mute | 有効 | - |
| controls | 有効 | - |
| loop | 有効 | playlist 必須 |
| playlist | 有効 | - |
| start / end | 有効 | - |
| playsinline | 有効 | - |
| enablejsapi | 有効 | - |
| modestbranding | 有効 | - |
| iv_load_policy | 有効 | - |
| cc_load_policy | 有効 | - |
| fs | 有効 | - |
| disablekb | 有効 | - |
| rel | 部分有効 | - |
| color | 部分有効 | - |
| showinfo | 廃止 | - |
| autohide | 廃止 | - |
| theme | 廃止 | - |
| version | 廃止 | - |
| rel=0（完全） | 廃止 | - |
| origin | 廃止 | - |

---

## 8. 注意
- jsDelivr はキャッシュされます（即時反映されない場合あり）  
- GitHack は表示・埋め込み用途向け  
- 最新性が必要な場合は GitHub Raw を推奨

---

# 9. README（英語版）

## about-youtube / youtubeeducation  
A complete reference for YouTube embedding, streaming, and alternative APIs.

### Notes
- Contact via Issues before using.  
- Include the repository URL where this data will be used.  
- Parameters and APIs update frequently (approx. every 2 days).

---

# 10. README（スペイン語版）

## about-youtube / youtubeeducation  
Referencia completa para la inserción de YouTube, transmisión y APIs alternativas.

### Notas
- Contacta por Issues antes de usar.  
- Incluye la URL del repositorio donde se utilizará.  
- Los parámetros y APIs se actualizan con frecuencia (aprox. cada 2 días).

---

# 11. README（オランダ語版）

## about-youtube / youtubeeducation  
Volledige documentatie voor YouTube-embedding, streaming en alternatieve API’s.

### Opmerkingen
- Neem contact op via Issues voordat je dit gebruikt.  
- Vermeld de repository-URL waar dit wordt toegepast.  
- Parameters en API’s worden vaak bijgewerkt (ongeveer elke 2 dagen).

---

# 12. README（中国語版 / 简体中文）

## about-youtube / youtubeeducation  
YouTube 嵌入、流媒体播放与替代 API 的完整参考文档。

### 注意事项
- 使用前请通过 Issues 联系。  
- 请注明使用此数据的仓库 URL。  
- 参数与 API 更新频繁（约每 2 天一次）。

---

# 13. README（韓国語版 / 한국어）

## about-youtube / youtubeeducation  
YouTube 임베드, 스트리밍, 대체 API에 대한 완전한 참고 문서입니다.

### 참고 사항
- 사용 전에 반드시 Issues로 연락해주세요.  
- 이 데이터를 사용할 저장소 URL을 명시해야 합니다.  
- 파라미터와 API는 자주 업데이트됩니다 (약 2일마다).

---

# 14. README（フランス語版 / Français）

## about-youtube / youtubeeducation  
Documentation complète pour l’intégration YouTube, le streaming et les API alternatives.

### Remarques
- Veuillez contacter via Issues avant utilisation.  
- Indiquez l’URL du dépôt où ces données seront utilisées.  
- Les paramètres et API sont mis à jour fréquemment (environ tous les 2 jours).

---

# 15. README（ドイツ語版 / Deutsch）

## about-youtube / youtubeeducation  
Umfassende Dokumentation zur YouTube-Einbettung, Streaming und alternativen APIs.

### Hinweise
- Bitte vor der Nutzung über Issues Kontakt aufnehmen.  
- Geben Sie die Repository-URL an, in der diese Daten verwendet werden.  
- Parameter und APIs werden häufig aktualisiert (ca. alle 2 Tage).

