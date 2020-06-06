# 静電容量Helixベータ ビルドガイド
## 静電容量Helixとは？
Helix Keyboardの基板を差し替え、静電容量スイッチに対応させる為のパーツです  
本家Helixとの共通部分については省略しています

## 注意
本キットは組み立て難易度が高く、使うパーツも特殊です。  
自作キーボードについて、最低限の知識があることを前提にドキュメントを書いています


## 対応スイッチ
下記のスイッチでのみ動作確認が取れています。  
Varmilo EC sakura  
Varmilo EC green  
Varmilo EC Rose  
  
通常のメカニカルスイッチでは動作しません
 
## 部品

下記は1つ作るのに必要な部品の数です。両手分を作るには2セット必要です。  

### 本家と共通の部品
| 名前 | 数 | 備考 |
| ---- | ---- | --- |
| Pro Micro | 1個 | |
| TRRSジャック | 1個 | |
| タクトスイッチ | 1個 | |
| スプリングピンヘッダ 12P | 2個 | コンスルーとも呼ばれています |
| プレート（アクリル） | 1セット| |
| 保護プレート | 1枚 | |
| M2スペーサー 7mm | 6個 |  |
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
| ジャンパ用の銅線 | 少し | | |

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

## 左右をジャンパ
絶縁テープの上から、写真のようにジャンパしていきます  
![image](https://user-images.githubusercontent.com/16838187/83893604-1d2cf600-a78b-11ea-9552-fb847786772a.png)

## 絶縁テープ
ジャンパの上に絶縁テープを貼ります  
![image](https://user-images.githubusercontent.com/16838187/83893829-73019e00-a78b-11ea-98b6-a781e42b639f.png)

## 裏側に各種パーツを実装する
基板をひっくり返し、各種パーツを実装します  
![ポンチ図](https://user-images.githubusercontent.com/16838187/83891190-c2de6600-a787-11ea-8927-8929d10d0dcb.png)

## その他のパーツを実装する
下記画像のパーツを実装していきます。  
片面にしかパッドがないため、  
右手側なら裏側に、左手側なら表側への実装となります  
![ポンチ図2](https://user-images.githubusercontent.com/16838187/83897147-29678200-a790-11ea-98a0-5f82ccec384a.png)  
![ポンチ図3](https://user-images.githubusercontent.com/16838187/83898727-443af600-a792-11ea-9359-abdeb232eadb.png)  

74HC4051DB　と オペアンプＡＤ８６１６ＡＲＭの向きには注意してください。  
また、熱に弱いためヒートクリップ等を使うことをおすすめします

## リセットスイッチ
本家と同じです。


## OLEDをつける(オプション)
本家と同じです

## backLightLEDをつける(オプション)
本家と同じです  
LEDテープによるunderglowには対応していません

## TRRSジャックをつける
両手分つくる場合は必要になります。  
本家と同じです

## スイッチソケットの実装
本家ではキースイッチを直接はんだ付けしていますが、  
こちらでははんだ付けせず、代わりにスイッチソケットをはんだ付けします。  
![image](https://user-images.githubusercontent.com/16838187/83894498-56199a80-a78c-11ea-884e-bf0ec07e8688.png)

## ProMicro
本家と同じです

## ProMicroにqmkを焼く
下記のファームウェアを焼く必要があります
https://github.com/ginjake/qmk_firmware/tree/ec_helix/keyboards/ec_helix

## トッププレート
トッププレートに静電容量スイッチをはめ込んだ後、スイッチソケットに入るように装着します。
このとき、スイッチの足が折れないように注意してください
## ボトムプレート
本家と同じです。  
ステンレスプレートでの動作は検証出来ていないので  
実験した方がいましたら教えて頂けると幸いです  
