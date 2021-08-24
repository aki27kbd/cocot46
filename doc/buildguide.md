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
|M2 スペーサー 8mm（メス―メス）|15本|寸法がシビアなため付属以外のものではプレートと干渉する可能性あり|
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
  ![bg_00_parts01](https://user-images.githubusercontent.com/88039287/127670585-35ee52b5-7d98-4b53-95de-14ae840451aa.jpg)

  〇付属品裏面
  ![bg_00_parts02](https://user-images.githubusercontent.com/88039287/127670641-f8c14711-227a-48bf-9c15-f7484efd1910.jpg)

  その他上述の「キット以外に必要なもの」および「オプション部品」を揃えた上で組み立てに取り掛かってください。

### 1. ダイオード

  PCB裏面に、写真の向きでダイオードをはんだ付けします。ダイオードの表面の線と、PCBのシルクの線の向きが揃うように配置してください。
  **ダイオードの向きは基板の左右で異なります。必ずシルクをよく確認した上ではんだ付けを行ってください。**
  予め片側にはんだを盛っておき、溶かしながらピンセットでダイオードを押さえつけると固定しやすくなります。  
  **全47箇所**はんだ付けを行ってください。
  ![bg_01_diode](https://user-images.githubusercontent.com/88039287/127675355-a4cb0ba7-0db6-4b36-bb3c-1e8090c5fc67.jpg)

### 2. MXソケット

  PCB裏面に、写真の向きでソケットをはんだ付けします。**全46箇所**はんだ付けを行ってください。
  ![bg_02_socket](https://user-images.githubusercontent.com/88039287/127672173-0f4f6359-dbe3-4662-87e5-a87ec42621b9.jpg)

### 3. タクトスイッチ

  PCB裏面に、タクトスイッチ（リセットスイッチ）をはんだ付けします。1箇所のみです。
  ![bg_03_reset](https://user-images.githubusercontent.com/88039287/127672408-63900b18-a897-4251-bb59-3364d8556370.jpg)

### 4. ProMicro

  ProMicroの準備をします。写真の向きでコンスル―をはんだ付けします。コンスル―には向きがあるので注意してください。マイクロUSBソケットはもげやすいので、適宜補強をしてからはんだ付けを行ってください。
  ![bg_04_promicro](https://user-images.githubusercontent.com/88039287/127672558-b29795b9-0192-4cca-91e0-c8eb80710140.jpg)

### 5. ロータリーエンコーダ

  中央部分にロータリーエンコーダをはんだ付けします。
  ### 写真

### 6. アンダーグロウLED（オプション）

  オプションでアンダーグロウLEDのはんだ付けを行います。PCBのシルク上の角の部分と、LEDの三角に欠けている部分の向きが揃うようにはんだ付けしてください。LEDは非常に熱に弱いので、はんだごての温度を低めに設定し、一か所はんだ付けをしたら十分時間をおいてから次のはんだ付けを行いましょう。
  ![bg_05_led](https://user-images.githubusercontent.com/88039287/127675025-0a87b3d8-4816-4ad1-829f-cc69e3e40dc6.jpg)

  LEDは下の写真の順番で取り付けましょう。
  ![bg_05_led02](https://user-images.githubusercontent.com/88039287/127674734-bda5f59c-24f2-45cc-b0f4-55e394c54d6a.jpg)

  全てのパーツを付け終わった状態です。
  ![bg_05_pcb](https://user-images.githubusercontent.com/88039287/127726727-5d338490-95d4-47cf-b4ea-5ae1db653376.jpg)

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
  ![bg_07_keyswitch](https://user-images.githubusercontent.com/88039287/127726620-1562592e-47df-4675-8b95-baf4d79f5e13.jpg)

### 9. 組み立て

  ProMicroをPCB表面に差し込みます。
  この段階で後述のファームウェアを準備し、問題なく動作しているか確認することをおすすめします。
  ![bg_08_assembly01](https://user-images.githubusercontent.com/88039287/127726946-f89ac4f3-d4fb-49d7-aac6-335a3235f702.jpg)

  キースイッチをはめたトッププレートをPCBにはめ込みます。
  ![bg_08_assembly02](https://user-images.githubusercontent.com/88039287/127726964-8bd3e6c0-59c8-472a-acbc-20d3dcbb668c.jpg)

  ねじとスペーサー（メス―オス）をトラックボール廻りの4箇所に固定します。
  ![bg_08_assembly03](https://user-images.githubusercontent.com/88039287/127727015-818ce255-7c71-4b7d-9c27-d931b4a0efc0.jpg)

  7で組み立てたトラックボールパーツをトラックボール固定プレートに通します。レベル変換基板を斜めにして通します。
  ![bg_08_assembly04](https://user-images.githubusercontent.com/88039287/127727084-da12b21a-e6a3-49e6-b9c0-d720cdc539b7.jpg)

  ケーブル部分を写真のように折りたたんでおきます。トラックボールの底面に両面テープを貼っておくと、後で位置固定がしやすくなります。
  ![bg_08_assembly05](https://user-images.githubusercontent.com/88039287/127727112-ec974f86-80cf-4fbe-b3fc-71b25a2001db.jpg)

  レベル変換基板のピンヘッダを、PCBにはんだ付けしたピンソケットに差し込みます。
  ![bg_08_assembly06](https://user-images.githubusercontent.com/88039287/127727127-2157f000-45d3-4742-8ba6-10685c621875.jpg)

  トラックボールを写真のように固定し、スペーサー（メス―メス）でトラックボール固定プレートを固定します。
  ![bg_08_assembly07](https://user-images.githubusercontent.com/88039287/127727180-5d8c45eb-9dec-434a-9a5a-7676d1d25524.jpg)

  穴の位置を合わせてトラックボールカバープレートを被せ、ねじ止めします。
  ![bg_08_assembly08](https://user-images.githubusercontent.com/88039287/127727200-db78c5a1-3c73-4da6-a884-0db6ee6d2932.jpg)

  ボトムプレートにスペーサーをねじ止めします。写真のように、上から見たときにリセットスイッチの穴の部分が左になるように固定します。赤丸の4箇所はオプションのアクリル積層ケースを組み立てる際に使用するものなので、無視してください。
  ![bg_08_assembly09](https://user-images.githubusercontent.com/88039287/127727382-6646a2cd-c8f9-4485-bc4d-e9d17028c8e7.jpg)

  最後にボトムプレートにPCB・スイッチプレートを被せ、11箇所ねじ止めします。ボトムプレートに6～7個のゴム足をバランスよく付ければ完成です。お好みのキーキャップを付けてご使用ください。
  ![bg_08_assembly10](https://user-images.githubusercontent.com/88039287/127727418-041633e2-0213-4d22-a231-d28f23a05b74.jpg)

### 10. アクリル積層ケース（オプション）

  下記パーツが揃っているかを確認します。
  ![bg_09_middle](https://user-images.githubusercontent.com/88039287/127728770-4426d20f-c63b-42b4-bd4d-a05063344a7b.jpg)

  シリコンシートのカッティング補助用に、[こちら](https://github.com/aki27kbd/cocot46/blob/main/doc/cocot46_silicon.pdf?raw=true)のシートをダウンロードし、**拡大率100%** で印刷してください。用紙に合わせて印刷してしまうとキースイッチの位置がずれてしまうのでご注意ください。
  印刷した型紙に、保護シートをはがしたシリコンシートを貼り付けます。ねじ部分は後からカットすることが難しいので、この状態で赤い部分のみカットしておきます。デザインナイフやカッターナイフ（30度刃）がカットしやすいと思います。
  ![bg_09_middle02](https://user-images.githubusercontent.com/88039287/127728987-2fab87eb-c4d3-4d76-aee1-35e03ea69b96.jpg)

  赤い部分をカットし終わったら、キースイッチの位置が合うようにミドルアクリルプレート（上）をシリコンシートの上に置き、外形（青線）とキースイッチ部分（灰色線）をカットしていきます。
  カットが終わった状態です。気泡が残っている場合は指で軽く押し出してください。
  ![bg_09_middle03](https://user-images.githubusercontent.com/88039287/127729808-50bf8ee0-dae8-47cd-827f-5da7b936f5be.jpg)

  ボトムプレート、ミドルプレート（下）PCB、ミドルプレート（上）、トッププレートの順に重ねます。
  ![bg_09_middle04](https://user-images.githubusercontent.com/88039287/127729839-f7f975fb-321d-4b66-b9b4-27f0bfca2e1e.jpg)

  ミドルプレートを装着する場合は、赤丸の部分に8mmのねじを用いてボトムプレートから直接PCB越しにスペーサーにねじ止めします。
  ![bg_09_middle05](https://user-images.githubusercontent.com/88039287/127729898-9eb1e454-1610-453e-9185-ace7f89ce32f.jpg)

  ミドルプレートを装着した場合の側面です。全体の剛性が増し、シリコンシートによって柔らかい打鍵感になります。隙間がなくなるので打鍵音も改善されます。
  ![bg_09_middle06](https://user-images.githubusercontent.com/88039287/127730012-13d8f4f7-3d61-40b0-b8f2-cde5f4a43956.jpg)

## ファームウェア

トラックボールを操作する手によって、2種類ファームウェアを用意しております。

[右手用](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_trackball_right.zip?raw=true)
[左手用](https://github.com/aki27kbd/cocot46/blob/main/firmware/cocot46_trackball_left.zip?raw=true)
.hexファイルをQMK ToolboxなどでProMicroに書き込めば、以降[ReMap](https://remap-keys.app/configure)でキーマップを変更することが可能です。

ソースコードは[こちら](https://github.com/aki27kbd/qmk_firmware/tree/master/keyboards/cocot46)を参照ください。

## 終わりに
何かトラブルがあれば[Twitterアカウント](https://twitter.com/aki27kbd)までご連絡ください。
また、完成写真をSNSにアップいただけるととても励みになります。
