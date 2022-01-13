# mypkg2
ロボットシステム学課題２のリポジトリ

# 使用機器
* PC(ubuntu20.04を使用)
* Rasberry Pi 3

# インストール
1. catkin_ws と src 2つのディレクトリを作成
2. ``` git@github.com:ReiYamaguchi59/mypkg2.git``` をクローンする
3. catkin_wsディレクトリでcatkin_make を実行

# 実行方法
以下のコマンドをUbuntuに入力する。

1.一つ目の端末でroscoreを起動
``` 
$ roscore &
```
2.一つ目の端末でcount.pyを走らせる
```
$ rosrun mypkg1 count.py
```
3.二つ目の端末でtwice.pyを走らせる
```
$ rosrun mypkg1 twice.py
```
4.三つ目の端末で動作の確認
```
$ rostopic echo /twice
```

※```$ rosrun```でノードの実行をする際、以下のパーミッション設定をする必要があります

```$ chmod +x count.py```
```$ chmod +x twice.py```
# ライセンス
BSD 3-Clause License
https://www.freebsd.org/ja/
