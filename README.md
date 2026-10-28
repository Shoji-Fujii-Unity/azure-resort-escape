# Azure月光リゾート — AZURE MOONLIGHT RESORT

[日本語](#日本語) · [English](#english)

> 廃墟になったシーサイドリゾートを舞台にした、単一HTMLファイルのポイント＆クリック脱出ゲーム。
> A point-&-click escape game set in an abandoned seaside resort, complete in a single HTML file.

---

## 日本語

### 概要

**Azure月光リゾート** は、インストール不要・オフライン動作のブラウザ脱出ゲームです。
`azure-resort-escape.html` をダブルクリックするだけで遊べます。

- **23の場所**：ロビー、受付、事務所、バー、売店、廊下・発電機室、大階段、客室201/205、キッチン、レストルーム、庭、プール、脱衣所、プールバー、ビーチ、海食洞、ボートガレージ、桟橋、灯台（外部・内部）
- **131の調査マーク**（日誌で進捗を確認できます）
- **約19種のアイテム**と組み立てギミック（懐中電灯＋UVライト、ボートの補修など）
- **解錠パズル4種**：3桁ダイヤル錠×2、バンド順当てはめ、オルゴール音符入力、ヒューズ盤
- **2つのエンディング**：脱出（ノーマル）／ 灯を再びともして出航（トゥルー）
- **日本語 / English 切り替え**（ゲーム中の全テキスト対応）
- **サウンド On/Off**：効果音・環境音はすべてWebAudioによる合成音（外部音声ファイルなし）
- **自動セーブ**：ブラウザの localStorage に保存（キー名 `azurescape_v1`）

### 遊び方

1. `azure-resort-escape.html` をブラウザで開く
2. タイトル画面で「**新規スタート**」（セーブがあれば「**続きから**」）
3. 画面内の**光るポイント**をタップ／クリックして調べる
4. 下段の**アイテムスロット**でアイテムを選び、使う場所でタップ
5. 画面端の**矢印**で移動（地図ボタンでも移動済み地点へダイレクト移動可）

**メニューボタン**

| ボタン | 役割 |
|---|---|
| 言語 | 日本語 ⇄ English |
| サウンド | 効果音・環境音の On/Off |
| 地図 | 発見済みの部屋へ一移動できる |
| 日誌 | 131マークの発見状況一覧 |
| ヒント | 今の状況に応じたヒントを表示 |
| 保存 | 手動セーブ（オートセーブあり） |
| タイトル | タイトル画面へ（セーブ済み） |

### スマホでの注意

- **横画面専用**です。縦画面では回転を促す画面が表示されます
- 画面比率16:9のレターボックス表示。ブラウザ全画面（F11）が最も大きく遊べます
- タッチ操作前提で、ホットスポットは長押しなしのタップで反応します

### 攻略の要点（ネタバレ注意！）

必要な番号はすべてゲーム内のどこかに書かれています。以下は最終解答例。

- **脱衣所の鍵番号：`427`**（ロビーの掲示板に手がかり）
- **事務所の金庫番号：`719`**（205号室の「暗い壁」にUVライトを当てると出現）
- **バーのジュークボックス**：バンド名を **Blue Moon → Sea Shell → Night Ferry → Anchor Man** の順にタップ（曲名「Azure Moon」の並び）
- **205号室のオルゴール**：テーマ曲 **C E G E C E**（201号室のラジオがヒントを演奏する）
- **ボート（ノーマルエンド）**：船体パッチ＝レジ引き出し（現金出納鍵は205のオルゴール）／エンジンキー＝金庫・プールスキマー（釣り竿で釣れる）／燃料＝ガレージの携行缶 → 桟橋で「**出航**」
- **発電機→トゥルーエンド**：キッチン冷蔵庫のヒューズ → 発電機室のヒューズ盤 → ガレージのオイル缶で給油 → 南京錠はバールで破壊→ブレーカーON → マッチで予熱→始動 → **灯台のメインスイッチ**（鍵は金庫の「LIGHT」刻印キー）→ 灯が点り、その後出航するとトゥルーエンド

ソフトロックには配慮済みです（主要な鍵・アイテムは二重の入手ルートあり）。

### セーブデータについて

- 保存先：`localStorage` の `azurescape_v1`（同じブラウザ・同じファイル位置なら再開可能）
- 初期化したい場合はタイトルで「新規スタート」を選ぶか、ブラウザのサイト設定からストレージを削除

---

## English

### Overview

**Azure Moonlight Resort** is a browser escape game that runs offline with no install —
just double-click `azure-resort-escape.html`.

- **23 locations**: lobby, reception, office, bar, store, corridors & generator room, grand staircase, guest rooms 201/205, kitchen, restrooms, garden, pool, changeroom, pool bar, beach, sea cave, boathouse, pier, lighthouse (outside & inside)
- **131 discoverable marks** (tracked in the journal)
- **~19 items** with combination gadgets (flashlight + UV lamp, boat repairs, …)
- **4 lock puzzles**: two 3-dial number locks, a band-order jukebox, a music-box note sequence, a fuse panel
- **Two endings**: escape (normal) / re-light the lighthouse and sail out (true)
- **日本語 / English** full text switching
- **Sound On/Off**: all SFX and ambience are synthesized with WebAudio (no audio files)
- **Autosave** to browser localStorage (key `azurescape_v1`)

### How to play

1. Open `azure-resort-escape.html` in any modern browser
2. On the title screen choose **NEW GAME** (or **CONTINUE** if a save exists)
3. Tap / click the **glowing spots** to investigate
4. Select an item from the **bottom slot bar**, then tap the place to use it
5. Walk through **arrow hotspots** at the screen edges (the Map button also teleports to visited rooms)

**Menu buttons**: language toggle · sound toggle · map (fast-travel to found rooms) ·
journal (mark checklist) · contextual hint · manual save · return to title.

### On phones

- The game is **landscape only**; a rotate prompt appears in portrait.
- The stage is a 16:9 letterboxed area — full-screen browser mode gives the biggest picture.
- Everything works with simple taps; no drag or long-press required.

### Walkthrough essentials (SPOILERS!)

Every code is written somewhere in the world. The final answers:

- **Changeroom locker code: `427`** (clue on the lobby notice board)
- **Office safe code: `719`** (shine the UV lamp on the dark wall in room 205)
- **Bar jukebox**: tap the bands in the order **Blue Moon → Sea Shell → Night Ferry → Anchor Man** (they spell the house hit "Azure Moon")
- **Room 205 music box**: play the resort theme **C E G E C E** (the radio in 201 hums the hint)
- **Boat (normal ending)**: hull patch = cash-register drawer (register key from the 205 music box) / engine key = safe, or fish it out of the pool skimmer with the rod / fuel = jerrycan in the boathouse → **SET SAIL** at the pier
- **Generator → true ending**: spare fuse (kitchen fridge) → fuse panel in the generator room → refuel with the boathouse oil can → cut the breaker padlock with the crowbar → breaker ON → pre-heat with matches → engine starts → throw the **lighthouse master switch** (key stamped "LIGHT" is in the safe) → the beam returns; sail out afterwards for the true ending

Soft-locks are prevented — every essential key/item has at least two ways to obtain it.

### Save data

- Stored in `localStorage` under `azurescape_v1` (resumes in the same browser / same file location)
- To reset: choose **NEW GAME** on the title screen, or clear the site's storage in browser settings

---

## 技術メモ / Technical notes

| | |
|---|---|
| 形式 / Format | 単一HTML（HTML+CSS+JS、外部アセットなし）/ single HTML file, zero external assets |
| 描画 / Graphics | インラインSVG（viewBox 1600×900、動的フラグでシーンが変化する）/ dynamic inline SVG scenes |
| 音 / Audio | WebAudio合成（オシレータ＋ノイズバースト）/ procedural oscillators + noise bursts |
| セーブ / Save | localStorage `azurescape_v1` |
| 検証 / Verified | Node.jsヘッドレスで全部屋描画・全ホットスポット動作・両エンド・セーブ往復を自動化テスト / automated headless smoke test of all rooms, hotspots, endings and save round-trip |
