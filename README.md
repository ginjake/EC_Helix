# 静電容量Helixベータ ビルドガイド
## 静電容量Helixとは？
Helix Keyboardの基板を差し替え、静電容量スイッチに対応させる為のパーツです
本家Helixとの共通部分については省略しています

## 部品

下記は1つ作るのに必要な部品の数です。両手分を作るには2セット必要です。

### 本家と共通の部品
| 名前 | 数 | 備考 |
| ---- | ---- | --- |
| Pro Micro | 1個 | |
| TRRSジャック | 1個 | |
| タクトスイッチ | 1個 | |
| スプリングピンヘッダ 12P | 2個 | 通常のピンヘッダでも可 |
| プレート（アクリル） | 1セット| |
| 保護プレート | 1枚 | |
| M2スペーサー 4mm | 6個 | ロープロファイルスイッチ用 |
| M2スペーサー 7mm | 6個 | MX互換スイッチ用 |
| M2スペーサー 8mm | 2個 | |
| M2ネジ 3mm| 14個 | |
| M2低頭ネジ 5mm| 2個 | |
| ゴム足 | 6個 |  |
| キーキャップ | 32個 | キースイッチと互換があるもの |
| 3.5mmオーディオケーブル | 左右合わせて1本 | 左右のキーボード接続用 |
| micro USBケーブル | 左右あわせて1本 | 
| SK6812mini | 32個 | バックライト用（オプション） |
| OLEDモジュール | 1個 | OLED用（オプション） |
| ピンソケット 4P | 1個 | OLED用（オプション） |
| ピンヘッダ 4P | 1個 | OLED用（オプション） |


### 本家と異なる部品
| 名前 | 数 | 備考 | 入手先 |
| ---- | ---- | --- | ---- |
| PCB | 1枚 | | |
| 静電容量キースイッチ | 32個 | Varmilo ECスイッチのみ対応 | |
| スイッチ用PCBソケット | 32個 | MX用 | https://yushakobo.jp/shop/a01ps/ |
| 1608(0603)チップ抵抗 100K | 7 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57HD |
| 1608(0603)チップ抵抗 10K | 2 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57GX |
| 1608(0603)チップ抵抗 1KΩ | 2| | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57GK |
| 1608(0603)チップ抵抗 200Ω | 6 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57FZ |
| 1608(0603)チップ抵抗 51KΩ | 1 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57H7 |
| 1608チップ積層セラミックコンデンサー 50Vdc 220pF | 1 | GRM1882C1H221JA01D*A (10個入り)| https://www.marutsu.co.jp/GoodsDetail.jsp?salesGoodsCode=19297&shopNo=3 |
|チップトランジスタ　２ＳＣ２７１２－ＧＲ　５０Ｖ１５０ｍ | 1 | | http://akizukidenshi.com/catalog/g/gI-00761/ |
| 74HC4051DB IC MUX/DEMUX 8X1 16SSOP | 1 | | https://www.marutsu.co.jp/pc/i/24340308/ |
| ２回路入オペアンプＡＤ８６１６ＡＲＭ | 1 | | http://akizukidenshi.com/catalog/g/gI-04570/ |


## 追加で必要な工具
| 名前 | 数 | 備考 | 入手先 |
| ---- | ---- | --- | ---- |
| ヒートクリップ | 1つ | | |
| 絶縁テープ | 1つ | | |



## 組み立て方
以降は左手用で説明します。右手用はPCBを反転して下さい。

__一度全ての工程を読み、理解してから作業を進めることをお勧めします。__

OLED,LED,TRRSジャック等のHelixの共通部分については省略します。
ただし、キースイッチは直接はんだづけしないでください

## 最初に絶縁テープを貼る
将来的にProMicroが刺さるところに絶縁テープを貼ります
![image](https://user-images.githubusercontent.com/16838187/83887616-a8a28900-a783-11ea-9be4-f0edcfd9118e.png)

## 裏側に各種パーツを実装する
基板をひっくり返し、各種パーツを実装します
![ポンチ図](https://user-images.githubusercontent.com/16838187/83891190-c2de6600-a787-11ea-8927-8929d10d0dcb.png)

74HC4051DB　と オペアンプＡＤ８６１６ＡＲＭの向きには注意してください。
また、熱に弱いためヒートクリップ等を使うことをおすすめします


