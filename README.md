# ros2_mypkg

![test](https://github.com/musashiharada/mypkg/actions/workflows/test.yml/badge.svg)

ロボットシステム学の練習リポジトリであり、このリポジトリはROS2のパッケージです。

## インストール方法
ターミナルに下記のように入力する。
```
$ git clone https://github.com/musashiharada/mypkg.git
```

## 機能
talkerで0から順に整数を数え、listenerでその数えた整数をそのまま出力する。

## 動作の仕方
Ubuntuの端末を二つ開き、一つのターミナルに下記のように入力する。
```
$ ros2 run mypkg talker　
```
もう一つのターミナルには下記のように入力する。
```
$ ros2 run mypkg listener　
```
listenerの方に以下のように出力される。
```
[INFO] [1671991971.177618000] [listener]: Listen: 0
[INFO] [1671991971.669417200] [listener]: Listen: 1
[INFO] [1671991972.169457200] [listener]: Listen: 2
[INFO] [1671991972.669297400] [listener]: Listen: 3
[INFO] [1671991973.169653400] [listener]: Listen: 4
[INFO] [1671991973.669616100] [listener]: Listen: 5
[INFO] [1671991974.169463200] [listener]: Listen: 6
[INFO] [1671991974.668907100] [listener]: Listen: 7
[INFO] [1671991975.169430600] [listener]: Listen: 8
[INFO] [1671991975.668671200] [listener]: Listen: 9
[INFO] [1671991976.169633600] [listener]: Listen: 10
```

またlaunchを使えば、一つの端末で動作確認することができる。
下記のようにターミナルに入力
```
$ ros2 launch mypkg  talk_listen.launch.py
```
以下のように出力される。
```
[listener-2] [INFO] [1671992183.194454600] [listener]: Listen: 0
[listener-2] [INFO] [1671992183.684191200] [listener]: Listen: 1
[listener-2] [INFO] [1671992184.184423100] [listener]: Listen: 2
[listener-2] [INFO] [1671992184.684597200] [listener]: Listen: 3
[listener-2] [INFO] [1671992185.184680100] [listener]: Listen: 4
[listener-2] [INFO] [1671992185.684633400] [listener]: Listen: 5
[listener-2] [INFO] [1671992186.184626800] [listener]: Listen: 6
[listener-2] [INFO] [1671992186.684521100] [listener]: Listen: 7
[listener-2] [INFO] [1671992187.183423600] [listener]: Listen: 8
[listener-2] [INFO] [1671992187.683907000] [listener]: Listen: 9
[listener-2] [INFO] [1671992188.184753100] [listener]: Listen: 10
```
## 必要なソフトウェア
* ROS2

## テスト環境
* Ubuntu 20.04 LTS

## ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます。
* © 2022 Musashi Harada

 
