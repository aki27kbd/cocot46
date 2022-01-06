# BMP Setup

![cocot46_bmp_top](https://user-images.githubusercontent.com/88039287/147035774-477be75d-5ef5-4a03-9b13-427cdebf269d.jpg)

cocot46をBLE Micro Proを用いて無線化する際はこちらを参照してください。



## 部品
### BMP化パーツセット

![cocot46_bmp_00_v2_rev](https://user-images.githubusercontent.com/88039287/147531155-6a36f926-293b-4446-82b2-1daaa11ad3e7.jpg)

|名前|数|備考|
|---|---|---|
|電池基板|1枚||
|単三電池ホルダー|1個||
|スライドスイッチ|2個||
|昇圧モジュール|1個||
|昇圧モジュール用ピンヘッダ|1個||
|コンデンサ|1個||
|ショットキーバリアダイオード|2個||
|L型ピンソケット（v1基板用）|1個||
|L型ピンヘッダ（v1基板用）|1個||
|5or6ピンコンスル―（v2基板用）|1個||
|トラックボール用ピンソケット|1個||

### セット以外に必要なもの

|名前|数|備考|
|---|---|---|
|BLE Micro Pro|1個||
|コンスルー（12本）|2本||
|単三電池|1本||

## 組み立て
### 1. パーツ実装

  〇裏面へのパーツ実装

  下の写真のように、電池基板の裏面に①ショットキーバリアダイオード×2個、②L型ピンソケットをはんだ付けします。  
  ショットキーバリアダイオードは向きに注意してください。

  ![cocot46_bmp_01](https://user-images.githubusercontent.com/88039287/147035884-3e25b082-29c8-4919-91e8-d504fa56bab1.jpg)

  〇表面へのパーツ実装

  下の写真のように、電池基板の表面に③単三電池ホルダー、④昇圧モジュール、⑤スライドスイッチ×2個、⑥コンデンサ、⑦ピンソケットをはんだ付けします。単三電池ホルダーの余分な足は切っておきましょう。  
  昇圧モジュールは付属のピンヘッダを切り離してはんだ付けします。表裏・向きに注意してはんだ付けを行ってください。  
  コンデンサには向きはありません。

  ![cocot46_bmp_02](https://user-images.githubusercontent.com/88039287/147035945-a2c7a61c-dae5-46be-9735-0157e4d4a08b.jpg)

### 2. 組み立て

  BLE Micro Proとコンスル―を写真のように固定します。（BLE Micro ProはProMicroと違ってはんだ付けをする必要がありません。）  
  キット付属の7mmスペーサ―（メス-メス）をPCBに固定します。

  ![cocot46_bmp_03](https://user-images.githubusercontent.com/88039287/147036230-7e91e26e-7b0a-4825-b558-66de94a0aa3e.jpg)

  ---

  <details><summary>【v1基板の場合】</summary><div>

  BLE Micro ProのBAT、GNDにピンヘッダをはんだ付けします。ピンヘッダは昇圧モジュールの付属のものの余りなどを用いてください。コンスル―を切り出せばはんだ付けせずとも電気的に接続できますが、接触不良を避けるためはんだ付けした方が確実です。

  ![cocot46_bmp_04](https://user-images.githubusercontent.com/88039287/147036255-956327bc-e775-4569-b0ab-0b5fadcdb292.jpg)

  L型ピンヘッダとL型ピンソケットを接続し、PCB上のトラックボール用ピンソケットに挿し込みつつ、BAT・GNDに固定したピンヘッダを電池基板の＋と－に通した上で、電池基板をスペーサ―の上に重ねます。電池基板の＋と－に通したピンヘッダをはんだ付けしてください。

  ![cocot46_bmp_05](https://user-images.githubusercontent.com/88039287/147036365-fccca06e-d3d8-4781-aad4-42648ebc32b4.jpg)

  </div></details>

  ---

  <details><summary>【v2基板の場合】</summary><div>

  PCB上の写真の箇所に、6ピンコンスル―を挿し込みます。  
  BMP用の12ピンコンスル―は写真の赤い箇所に設置してください。

  ![cocot46_bmp_04_v2_rev](https://user-images.githubusercontent.com/88039287/148387927-e90485e0-ab76-4d46-9d1b-d1beb1c16268.jpg)

  6ピンコンスル―を電池基板に通した上でスペーサ―の上に重ねます。

  ![cocot46_bmp_05_v2](https://user-images.githubusercontent.com/88039287/147530119-e91da06b-9698-4787-9535-5fa799994163.jpg)

  </div></details>

  ---

  キット付属の8mmスペーサ―（メス-オス）で電池基板を固定します。トラックボールレベル変換基板のピンを電池基板上のソケットに挿し込みます。スペーサーの高さが変わるため、トラックボールが少し浮いてしまう場合があります。厚手の両面テープ等をトラックボールの裏面に貼ることで適宜高さを調整してください。

  ![cocot46_bmp_06](https://user-images.githubusercontent.com/88039287/147036399-5d612f64-c00e-4a6e-880f-bfa2848eb981.jpg)

  最後にトラックボールカバープレートを付けて完成です。

  ![cocot46_bmp_07](https://user-images.githubusercontent.com/88039287/147036454-5ade8b1f-ff57-4be4-9fc2-85d78a9b6717.jpg)

  左側のスライドスイッチは電池のON・OFFを操作可能です。  
  右側のスライドスイッチはトラックボールへの給電を電池/USBで切り替えられるようになっています。  
  無線接続の場合はBAT側に、USB接続の場合はUSB側にスライドしてください。

  ![cocot46_bmp_08](https://user-images.githubusercontent.com/88039287/147037079-48a0db5c-a4de-4aa0-b352-129093c0bb7d.jpg)

## ファームウェア

BLE Micro Proに[Web Configurator](https://sekigon-gonnoc.github.io/BLE-Micro-Pro-WebConfigurator/)から最新のブートローダ・アプリケーションを書き込みます。手順は[こちら](https://sekigon-gonnoc.github.io/BLE-Micro-Pro/#/getting_started?id=%e3%83%95%e3%82%a1%e3%83%bc%e3%83%a0%e3%82%a6%e3%82%a7%e3%82%a2%e3%81%ae%e3%82%a2%e3%83%83%e3%83%97%e3%83%87%e3%83%bc%e3%83%88)を参照してください。

次にブートローダを起動してファームを書き込みます。詳細は[こちら](https://sekigon-gonnoc.github.io/BLE-Micro-Pro/#/build_firmware?id=%e7%94%9f%e6%88%90%e3%81%97%e3%81%9f%e3%83%95%e3%82%a1%e3%83%bc%e3%83%a0%e3%82%a6%e3%82%a7%e3%82%a2%e3%82%92%e6%9b%b8%e3%81%8d%e8%be%bc%e3%82%80)を参照してください。

書き込むuf2ファイルは[こちら](https://github.com/aki27kbd/cocot46/blob/main/firmware/BMP/cocot46_default.zip?raw=true)をご利用ください。

### ファームウェアカスタマイズ

#### CONFIG.JSN

CONFIG.JSNの設定により、動作をカスタマイズできます。

- peripheral

    ```
    "peripheral":{"max_interval":20,"min_interval":10,"slave_latency":7},
    ```
    - 通信間隔の設定です。短くすると入力のラグが減りtrack ballのカクつきを抑えることができますが、電力消費が増加します。

- reserved [3] ---- track ball angle
    ```
    "reserved":[0,0,0,7,3,0,0,0]}}
                      |
    ```
    - track ballを動かした際のカーソルの動作角度をずらします。
    - 0〜120の範囲で設定して下さい。
    - 1大きくすると時計回りに3度ずれます。\
      7を指定すると右に21度、100を指定すると右に300度（=左に60度）回転します。
    - track ballを右手で操作する方は15(右に45度)、左で操作する方は105(右に315度=左に45度)くらいに設定すると自然な動きになります。お好みで調整して下さい。

- reserved [4] ---- track ball speed
    ```
    "reserved":[0,0,0,7,3,0,0,0]}}
                        |
    ```
    - track ballの動作速度を設定します。
    - 0(遅い）〜5(速い)の範囲で設定して下さい。


#### ENCODER.JSN

- Remapでキーコード設定をできるようにするため、ENCODER.JSONにダミーのカスタムキーコードを設定しておいてkeymap.cの方でRemapで設定されたキーコードが入力されるようにしています。
- 以下の設定ではLayler1〜3まででエンコーダの操作が有効になります。
```
{"pin":[7,8],"step":1,"action":[["ANY(24000)","ANY(24001)"], ["ANY(24000)","ANY(24001)"], ["ANY(24000)","ANY(24001)"], ["KC_NO","KC_NO"], ["KC_NO","KC_NO"]]}
]}}
```
