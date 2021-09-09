# Build Guide

![cocot46_bg_00](https://user-images.githubusercontent.com/88039287/130355466-f4b49741-5ca4-40cb-bde0-aaf9d45f38c8.jpg)

cocot46のビルドガイドになります。
cocot46は中央に1uトラックボールを備えていることが一つの特徴です。
また親指キーの中央にロータリーエンコーダを配置しており、ホームポジションを崩すことなく両手の親指でエンコーダの操作が可能となっています。
その他オプションとしてアンダーグロウLED、アクリル積層ケースを用意しているので、お好みに合わせて実装ください。

## 部品
### キット付属品
|名前|数|備考|
|---|---|---|
|PCB|1枚||
|トッププレート（FR4）|1枚||
|ボトムプレート（アクリル）|1枚||
|トラックボールカバープレート（FR4）|1枚||
|トラックボール固定プレート（FR4）|1枚||
|M2 スペーサー 8mm（メス―メス）|11本|寸法がシビアなため付属以外のものではプレートと干渉する可能性あり|
|M2 スペーサー 7mm（メス―メス）|4本||
|M2 スペーサー 8mm（メス―オス）|4本||
|M2 ねじ 4mm|30本||

### キット以外に必要なもの

全てのパーツは[遊舎工房](https://shop.yushakobo.jp/)で揃えることが可能です。

|名前|数|備考|
|---|---|---|
|MicroUSBケーブル|1本||
|タクトスイッチ|1個||
|ゴム足|6～7個||
|ProMicro（コンスル―付）|1個||
|ダイオード|47個|SMD部品のみ対応、**ダイオードのみ46個ではなく47個必要なのでご注意ください。**|
|MXソケット|46個||
|キースイッチ|46個|MX互換|
|キーキャップ|46個|MX互換|
|ロータリーエンコーダ|1個||
|7mmオプティカルトラックボールモジュール１uタイプ|1個||
|トラックボールモジュール用レベル変換基板|1個||
|OLED用ピンソケット|1個||
|OLED用ピンヘッダ|1個||
|フルカラーシリアルLED (WS2812B)|10個|アンダーグロウ用（オプション）|

7㎜オプティカルトラックボールモジュール1uタイプに関しては[Amazon](https://www.amazon.co.jp/BitTradeOne-ADTB7M-7mm%E3%82%AA%E3%83%97%E3%83%86%E3%82%A3%E3%82%AB%E3%83%AB%E3%83%88%E3%83%A9%E3%83%83%E3%82%AF%E3%83%9C%E3%83%BC%E3%83%AB%E3%83%A2%E3%82%B8%E3%83%A5%E3%83%BC%E3%83%AB%EF%BC%91u%E3%82%BF%E3%82%A4%E3%83%97/dp/B087BVNWYS)、[モノタロウ](https://www.monotaro.com/p/6295/7835/)でも購入可能です。

トラックボールモジュール用レベル変換基板に関しては[のぎすけ屋様](https://nogikes.booth.pm/items/2008258)でも購入可能です。

各ショップの在庫状況に応じて検討ください。

### オプション部品（アクリル積層ケース）

アクリルは[遊舎工房](https://shop.yushakobo.jp/)などのレーザーカットサービスでお好きな色のアクリルプレートを発注することが可能です。
シリコンシートは[こちら](https://www.monotaro.com/p/3629/5253/)から購入可能です。

|名前|数|備考|
|---|---|---|
|アクリルミドルプレート（上）|1枚|アクリル積層ケース用|
|アクリルミドルプレート（下）|1枚|アクリル積層ケース用|
|シリコンシート厚さ0.5mm|1枚|アクリル積層ケース用|
|M2 ねじ 8mm|4本||

## 組み立て
### 0. 部品確認

  まずはパーツが揃っているか確認ください。

  〇付属品表面

  ![cocot46_bg_00_1](https://user-images.githubusercontent.com/88039287/131105567-73eda270-b10d-4c8a-a571-b01e3da3070e.jpg)

  〇付属品裏面

  ![cocot46_bg_00_2](https://user-images.githubusercontent.com/88039287/131105664-c0717bb6-ff4b-4e9a-80e2-2cc333f1a82f.jpg)

  その他上述の「キット以外に必要なもの」および「オプション部品」を揃えた上で組み立てに取り掛かってください。

### 1. ダイオード

  PCB裏面に、写真の向きでダイオードをはんだ付けします。ダイオードの表面の線と、PCBのシルクの線の向きが揃うように配置してください。
  **ダイオードの向きは基板の左右で異なります。必ずシルクをよく確認した上ではんだ付けを行ってください。**
  予め片側にはんだを盛っておき、溶かしながらピンセットでダイオードを押さえつけると固定しやすくなります。  
  **全47箇所**はんだ付けを行ってください。

  左手側裏面のダイオードの向き

  ![cocot46_bg_01_diode_1](https://user-images.githubusercontent.com/88039287/130643462-a7fda493-d140-46f5-87ce-5d243abccfc5.jpg)

  右手側裏面のダイオードの向き

  ![cocot46_bg_01_diode_2](https://user-images.githubusercontent.com/88039287/130643598-73b590ef-5cef-4716-b62e-902fa79e9572.jpg)


### 2. MXソケット

  PCB裏面に、写真の向きでソケットをはんだ付けします。**全46箇所**はんだ付けを行ってください。

  ![cocot46_bg_02_socket_1](https://user-images.githubusercontent.com/88039287/130643875-2290041c-98fb-442f-a8b0-72ac9785b679.jpg)

### 3. タクトスイッチ

  PCB裏面に、タクトスイッチ（リセットスイッチ）をはんだ付けします。1箇所のみです。

  ![cocot46_bg_03_reset_1](https://user-images.githubusercontent.com/88039287/130644608-b83a9835-7b28-4ad3-9ed3-a5eb7a4702c4.jpg)

### 4. ProMicro

  ProMicroの準備をします。写真の向きでコンスル―をはんだ付けします。コンスル―には向きがあるので注意してください。マイクロUSBソケットはもげやすいので、適宜補強をしてからはんだ付けを行ってください。

  ![bg_04_promicro](https://user-images.githubusercontent.com/88039287/127672558-b29795b9-0192-4cca-91e0-c8eb80710140.jpg)

### 5. ロータリーエンコーダ

  中央部分にロータリーエンコーダをはんだ付けします。ロータリーエンコーダの脚を通し、裏側からはんだ付けをしてください。

  ※オプションのアクリル積層ケースを付ける場合、ロータリーエンコーダの脚とのクリアランスがギリギリとなっています。特に上側の2本と下側の3本は脚の内側から最小限のはんだで固定するようご注意ください。

  ![cocot46_bg_05_re_1](https://user-images.githubusercontent.com/88039287/130783341-095f08a0-6e07-4d2e-b3ba-bb184185bc34.jpg)

  ![cocot46_bg_05_re_2](https://user-images.githubusercontent.com/88039287/130783531-b107372b-1bf9-470e-8eb4-71a48c22b847.jpg)


### 6. アンダーグロウLED（オプション）

  オプションでアンダーグロウLEDのはんだ付けを行います。PCBのシルク上の角の部分と、LEDの三角に欠けている部分の向きが揃うようにはんだ付けしてください。LEDは非常に熱に弱いので、はんだごての温度を低めに設定し、一か所はんだ付けをしたら十分時間をおいてから次のはんだ付けを行いましょう。  
  この段階で後述のファームウェアを準備し、LEDの点灯を一つずつ確認しながらはんだ付けを行うとミスの早期発見につながります。

  ![cocot46_bg_06_led_1](https://user-images.githubusercontent.com/88039287/131107120-fa2f57f8-0d3c-417c-a00a-f6e250911660.jpg)

  LEDは下の写真の順番で取り付けましょう。

  ![cocot46_bg_06_led_2](https://user-images.githubusercontent.com/88039287/130645118-b605c2cd-e3ad-4596-83f3-7d9b20aa88a5.jpg)

  全てのパーツを付け終わった状態です。

  ![cocot46_bg_06_led_3](https://user-images.githubusercontent.com/88039287/130783780-602c0f55-8cb0-4651-846f-f4625658b9ff.jpg)

### 7. トラックボール

  トラックボール装着に必要なパーツ一覧です。
  ![bg_06_trackball01](https://user-images.githubusercontent.com/88039287/127732488-2006694b-4cd9-4ecb-84d5-657a4e47890d.jpg)

  写真のように、PCB表面からピンソケットを差し込み、ずれないようにマスキングテープなどで固定します。裏返してPCB裏面からはんだ付けを行ってください。
  ![bg_06_pinsocket](https://user-images.githubusercontent.com/88039287/127726804-fd0f6cfb-cb91-444d-8eaf-f58504fb5220.jpg)

  次にトラックボールモジュールとレベル変換基板、ピンヘッダとレベル変換基板を下の写真のようにはんだ付けしてください。
  ![bg_06_trackball02](https://user-images.githubusercontent.com/88039287/127732522-2493b0ef-5bc0-43aa-bba3-e032b3b33e50.jpg)

  ![bg_06_trackball03](https://user-images.githubusercontent.com/88039287/127732530-8cbf2eb8-3d85-49f9-9950-76b7d5b5c819.jpg)

  こちらのパーツは9の組み立ての際に使用します。

### 8. キースイッチ

  トッププレートにキースイッチをはめ込みます。少しきつい部分もあるので、先にある程度スイッチをはめておいた方が後でプレートがたわみにくいです。

  ![cocot46_bg_08_switch](https://user-images.githubusercontent.com/88039287/130783959-4dce844e-4ee1-48d1-afe2-4e894ac62c3d.jpg)

### 9. 組み立て

  ProMicroをPCB表面に差し込みます。
  LEDを未実装の場合はこの段階で後述のファームウェアを準備し、問題なく動作しているか確認することをおすすめします。

  ![cocot46_bg_09_assembly_1](https://user-images.githubusercontent.com/88039287/130784074-3ca541e8-623d-4d13-92ac-c71e1d1d6b8b.jpg)

  キースイッチをはめたトッププレートをPCBにはめ込みます。

  ![cocot46_bg_09_assembly_2](https://user-images.githubusercontent.com/88039287/130784185-8bb1026f-f219-47c1-b7dd-50ff1e0d42dc.jpg)

  ねじとスペーサー（メス―オス）をトラックボール廻りの4箇所に固定します。

  ![cocot46_bg_09_assembly_3](https://user-images.githubusercontent.com/88039287/130784292-52b624e9-d62b-40f2-8d37-f0e80d202c17.jpg)

  7で組み立てたトラックボールパーツをトラックボール固定プレートに通します。レベル変換基板を斜めにして通します。

  ![cocot46_bg_09_assembly_4](https://user-images.githubusercontent.com/88039287/130784379-0bafdbaa-24c1-4a3b-aa4e-d61578f78c43.jpg)

  ケーブル部分を写真のように折りたたんでおきます。トラックボールの底面に両面テープを貼っておくと、後で位置固定がしやすくなります。

  ![bg_08_assembly05](https://user-images.githubusercontent.com/88039287/127727112-ec974f86-80cf-4fbe-b3fc-71b25a2001db.jpg)

  レベル変換基板のピンヘッダを、PCBにはんだ付けしたピンソケットに差し込みます。

  ![cocot46_bg_09_assembly_5](https://user-images.githubusercontent.com/88039287/130784491-cda776ca-77b0-446a-a578-57eecee166f6.jpg)

  トラックボールを写真のように固定し、スペーサー 7mm（メス―メス）でトラックボール固定プレートを固定します。**スペーサ― 8mm（メス―オス）と同封されている短い方のスペーサ―をお使いください。**

  ![cocot46_bg_09_assembly_6](https://user-images.githubusercontent.com/88039287/130784685-39ba0ab4-d931-446b-aa44-442c5501a785.jpg)

  穴の位置を合わせてトラックボールカバープレートを被せ、ねじ止めします。

  ![cocot46_bg_09_assembly_7](https://user-images.githubusercontent.com/88039287/130784863-92cadb26-416c-46b3-9eda-184f803ec7f6.jpg)

  ボトムプレートに**スペーサー 8mm（メス―メス）**をねじ止めします。写真のように、上から見たときにリセットスイッチの穴の部分が左になるように固定します。赤丸の4箇所はオプションのアクリル積層ケースを組み立てる際に使用するものなので、無視してください。

  ![cocot46_bg_09_assembly_8](https://user-images.githubusercontent.com/88039287/130785207-594bdb99-de80-4699-8c12-765f67f789f7.jpg)

  最後にボトムプレートにPCB・スイッチプレートを被せ、11箇所ねじ止めします。ボトムプレートに6～7個のゴム足をバランスよく付ければ完成です。お好みのキーキャップを付けてご使用ください。

  ![cocot46_bg_09_assembly_09](https://user-images.githubusercontent.com/88039287/130785293-ea786937-3f29-4e86-a3d1-d43d7a310c4f.jpg)

### 10. アクリル積層ケース（オプション）

  オプションであるアクリル積層ケースの組み立て方についてです。
  下記パーツを揃えた上で積層ケースの組み立てにのぞんでください。

  |名前|数|備考|
  |---|---|---|
  |アクリルミドルプレート（上）|1枚|※1|
  |アクリルミドルプレート（下）|1枚|※1|
  |シリコンシート 厚さ0.5mm|1枚|[こちら](https://www.monotaro.com/p/3629/5253/)から購入可能|
  |M2ねじ 8mm|4本||

  ※1 アクリルプレートは[こちらのデータ](https://github.com/aki27kbd/cocot46/blob/main/doc/cocot46_middle_plate.zip?raw=true)を用いて各自で用意ください。.aiデータは[遊舎工房のアクリルカットサービス](https://shop.yushakobo.jp/collections/services-auto/products/lasercut)に適合したデータ形式となっていますので、そのまま発注いただくことが可能です。
  お好みのカラーで**厚さ3㎜・A4サイズ**を指定して発注するようにしてください。
  ![cocot46_middle_A4](https://user-images.githubusercontent.com/88039287/130648054-da44450a-68ae-4e35-aa60-881c3b8859ee.jpg)

  シリコンシートのカッティング補助用に、[こちら](https://github.com/aki27kbd/cocot46/blob/main/doc/cocot46_silicon.pdf?raw=true)のシートをダウンロードし、**拡大率100%** で印刷してください。用紙に合わせて印刷してしまうとキースイッチの位置がずれてしまうのでご注意ください。
  印刷した型紙に、保護シートをはがしたシリコンシートを貼り付けます。ねじ部分は後からカットすることが難しいので、この状態で赤い部分のみカットしておきます。デザインナイフやカッターナイフ（30度刃）がカットしやすいと思います。

  ![cocot46_bg_10_middleplate_2](https://user-images.githubusercontent.com/88039287/130648308-ddf3674a-893e-4545-9321-22481a59c4da.jpg)

  赤い部分をカットし終わったら、キースイッチの位置が合うようにミドルアクリルプレート（上）をシリコンシートの上に置き、外形（青線）とキースイッチ部分（灰色線）をカットしていきます。

  ボトムプレート、ミドルプレート（下）PCB、ミドルプレート（上）、トッププレートの順に重ねます。

  ![cocot46_bg_10_middleplate](https://user-images.githubusercontent.com/88039287/130785781-7379371b-4250-44ac-9607-b6eaacc8f82e.jpg)

  ミドルプレートを装着する場合は、赤丸の部分に8mmのねじを用いてボトムプレートから直接PCB越しにスペーサーにねじ止めします。

  ![cocot46_bg_10_middleplate_3](https://user-images.githubusercontent.com/88039287/130786145-61ae336f-8697-4be1-baa6-329f61732c3d.jpg)

  ミドルプレートを装着した場合の側面です。全体の剛性が増し、シリコンシートによって柔らかい打鍵感になります。隙間がなくなるので打鍵音も改善されます。

  ![cocot46_bg_10_middleplate_4](https://user-images.githubusercontent.com/88039287/130786227-e414efee-9b78-4da8-b7c5-9e65659057dd.jpg)

## ファームウェア

トラックボールを操作する手によって、2種類ファームウェアを用意しております。

[右手用](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_trackball_right.zip?raw=true)

[左手用](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_trackball_left.zip?raw=true)

.hexファイルをQMK ToolboxなどでProMicroに書き込めば、以降[ReMap](https://remap-keys.app/configure)でキーマップを変更することが可能です。トラックボール、LED含めて上記.hexファイルで確認いただけます。

![remap](https://user-images.githubusercontent.com/88039287/130786498-4202abef-06bf-4c86-a5e6-c8a95990caf2.jpg)

組み立て段階で動作確認をする際も、ReMapのTest Matrix Modeを使うと便利です。

ソースコードは[こちら](https://github.com/aki27kbd/qmk_firmware/tree/master/keyboards/cocot46)を参照ください。

## 終わりに
何かトラブルがあれば[Twitterアカウント](https://twitter.com/aki27kbd)までご連絡ください。

また、完成写真をSNSにアップいただけるととても励みになります。（アップするのがはばかられる方はDMで直接送りつけていただいても構いません。）

ハッシュタグは #cocot46 です。
