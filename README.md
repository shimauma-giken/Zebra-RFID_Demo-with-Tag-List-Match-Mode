#### Zebra-RFID_Demo with Tag List Match Mode
## Tag List Match Mode(棚卸しモード）でデモする手順

2026年9月6日

### 概要
この記事では、Tag List Match Mode(棚卸しモード）でデモする手順を説明します。

### 必要なマテリアル
- Zebra Android端末
- Zebra RFID ハンドヘルドリーダ (RFDシリーズ、TC22R、MC33_Rシリーズ)

### デモ準備

#### 1. Tag List Match Mode用のファイルを作成

1. 下記説明文を参考にCSVファイルを作成します。


    - csv構成

    |||
    |-|-|
    |第１カラム | EPC
    |第２カラム | アイテム名

    * ヘッダ情報は不要です。<br/>
    * UTF-8 フォーマットで保存ください。
    
    <br/>

    - csv 例
    ```
    30352E5FC4261B263063C0EF,伸縮絆創膏
    30352E5FC4261B263063C0EA,伸縮絆創膏
    30353062CC0320A63063C0EC,サージカルテープ
    30352FADDC298EE6306380E5,体温計OMRON
    30353062180449A6306340E4,スローソフトS
    30353062500ACBE6306380E9,トラベルミン
    30352E5FC42711A63063C0EB,ワントップゲル
    ....
    ```

    [サンプルcsv](./99box.csv)

<br/>

#### 2. CsvファイルをAndroid端末に転送

1. 下記リンクを参考に、作成したcsvをAndroid端末に転送します。<br/>
   [コンピュータとAndroid デバイス間のファイル転送を有効にする](https://github.com/shimauma-giken/Zebra-Android_Transfer-Files-Between-Computer-and-Android-Device)


#### 123RFIDの操作

1. Google Play 経由で123RFID Mobile をインストールします。
2. 123RFIDにてリーダーに接続します。
3. [Settings] > [Application] > [Tag List Match Mode]を選択します。

   <img width="250px" src=".\image-4.png">
    <br/>   
4. 上記手順で作成したcsvファイルを選択します。
    <img width="250px" src=".\image-1.png">
    <br/>
1. [RFID] タブを選択し、読み取りを開始すると、Tag List Match Modeでインベントリを開始します。
   - **画像右**：左上のロケットアイコンを選択することで**Rapid**画面になります。
   - **画像左**：右上のロケットアイコンを選択することで**Invntory**画面になります。検知済みは緑表示、未検知は赤表示になります。
    <br/>

    <img width="250px" src=".\image-2.png"> <img width="250px" src=".\image-3.png">
    <br/>

### 備考


その他設定の詳細については、[123RFID Mobile Application User Guide](https://www.zebra.com/jp/ja/support-downloads/software/rfid-software/123rfid-mobile.html#Ta-item-7e5a553b68-tab)を参照してください。

-- end