
センサモデルの追加方法
===============================

Unity Sensorsパッケージのインストール方法
------------------------------------------

１．ショベル実機のＩＭＵセンサの取り付け位置確認

シミュレーション対応の実機についてＩＭＵセンサの取り付け位置を
写真などにて確認する（例：zx120）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-1 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/IMG_2394.jpg
          :scale: 100%
          :height: 100px
          :width: 200px
     - 実機写真を参考に取り付け位置を確認する

ＩＭＵセンサは、zx120ショベルの場合、swing、boom、arm、bucket　が存在する

２．UnitySensors パッケージのインストール

ＩＭＵセンサを作成する前準備としてUnitySensors パッケージを追加インストールする

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-2 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-02.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity メニューバーから「Windows」「Package Manager」を選択する

３．Package Manager ウィンドウのメニューバーから「＋」「Add package from git URL」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-3 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-03.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Manager ウィンドウ
   * - .. image:: imu_gnss/img/unity-04.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - メニューバーから「＋」「Add package from git URL」を選択する

４．Package Manager ウィンドウのＵＲＬ入力テキストボックスに下記のURLを入力し「Add」ボタンを押下する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-06.png
          :scale: 100%
          :height: 150px
          :width: 400px
     - Package Manager ウィンドウのＵＲＬ入力テキストボックスに下記のURLを入力し「Add」ボタンを押下する
   * - 入力するURL【※１】
     - "https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensors#v2.0.4"

【※１】注意：Package のバージョンについては、記載時以降にバージョンアップされる場合があります
　下記のURL にて最新バージョンを確認の上対応のPackage についてURLを入力してください
　Assets/UnitySensors　https://github.com/Field-Robotics-Japan/UnitySensors

５．UnitySensors パッケージがインストールされる

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-5 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-07.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensors パッケージがインストールされる

６．UnitySensors パッケージがインストールされたことを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-6 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-08.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensors パッケージがインストールされたことを確認する

７．Package Manager ウィンドウのメニューバーから再度、「＋」「Add package from git URL」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-7-a　図 1-7-b　[拡大] 
     - 操作
   * - .. image:: imu_gnss/img/unity-03.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Manager ウィンドウ
   * - .. image:: imu_gnss/img/unity-04.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - メニューバーから再度、「＋」「Add package from git URL」を選択する

８．Package Manager ウィンドウのＵＲＬ入力テキストボックスに下記のURLを入力し「Add」ボタンを押下する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-8 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-09.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Manager ウィンドウのＵＲＬ入力テキストボックスに下記のURLを入力し「Add」ボタンを押下する
   * - 入力するURL【※２】
     - "https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensorsROS#v2.0.4" 

【※２】注意：Package のバージョンについては、記載時以降にバージョンアップされる場合があります
　下記のURL にて最新バージョンを確認の上対応のPackage についてURLを入力してください
　Assets/UnitySensors　https://github.com/Field-Robotics-Japan/UnitySensors

９．UnitySensorsROS パッケージがインストールされる

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-9 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-10.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensorsROS パッケージがインストールされる

10．UnitySensorsROS パッケージがインストールされたことを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-10 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-11.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensorsROS パッケージがインストールされたことを確認する

IMUセンサモデルの追加方法
--------------------------

１．Unity Editorで空オブジェクトCreate Emptyの作成

Unity Editor を起動し、ＩＭＵの空オブジェクトを作成する（例：boom_imu の場合）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　2-1 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity editorを起動する
   * - .. image:: /imu_gnss/img/unity-01-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity 「Hierarchy」タブから「zx120」「base_link」「body_link」「boom_link」を選択し右クリックで「Create Empty」を選択する

boom_imu の場合、ショベルの実機写真（図　1-1 ）からショベルモデルのboom_link から空オブジェクトを作成する

２．「Inspector」タブで GameObjectに名称を設定する（例：boom_imu）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　2-2 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-02-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - GameObjectに名称を設定する（例：boom_imu）


３．unity 「Hierarchy」タブから「boom_imu」を選択し「Inspector」タブを参照する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-3 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-15.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity 「Hierarchy」タブから「boom_imu」を選択し「Inspector」タブを参照する

４．「Inspector」タブから「Add Component」ボタンを押下し「IMU Sensor」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-16.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブから「Add Component」ボタンを押下し「IMU Sensor」を選択する

５.「IMU Sensor」のコンポーネントが「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-5 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-17.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「IMU Sensor」のコンポーネントが「Inspector」タブに追加されていることを確認する

６.再度「Inspector」タブから「Add Component」ボタンを押下し「IMU Msg Publisher 」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-6 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-18.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 再度「Inspector」タブから「Add Component」ボタンを押下し「IMU Msg Publisher 」を選択する

７.「IMU Msg Publisher」のコンポーネントが「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-7 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-19.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「IMU Msg Publisher」のコンポーネントが「Inspector」タブに追加されていることを確認する

８.「Inspector」タブを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-8 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-20.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブを確認する

９.unity のPlay ボタンを選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-9 
     - 操作
   * - .. image:: imu_gnss/img/unity-21.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity のPlay ボタンを選択する

10.「Inspector」タブがデータ更新されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-10 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-22.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブがデータ更新されていることを確認する

同様の方法で、swing、arm、bucket についてＩＭＵセンサモデルを追加する

GNSSセンサモデルの追加方法
--------------------------

１．ショベル実機のＧＮＳＳセンサの取り付け位置確認

シミュレーション対応の実機についてＧＮＳＳセンサの取り付け位置を
写真などにて確認する（例：zx120）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-1 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/GNSS-01.jpg
          :scale: 100%
          :height: 100px
          :width: 200px
     - 実機写真を参考に取り付け位置を確認する

ＧＮＳＳセンサは、実機写真からショベルモデルの　body部分に設定されていることを確認する 


２．Unity Editorで空オブジェクトCreate Emptyの作成

Unity Editor を起動し、ＧＮＳＳの空オブジェクトを作成する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-2 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity editor を起動する
   * - .. image:: /imu_gnss/img/gnss-02.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity 「Hierarchy」タブから「zx120」「base_link」「body_link」を選択し右クリックで「Create Empty」を選択する

２．「Inspector」タブで GameObjectに名称を設定する（例：gnss）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-3 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-04.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - GameObjectに名称を設定する（例：gnss）


３．unity 「Hierarchy」タブから「gnss」を選択し「Inspector」タブを参照する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-05.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity 「Hierarchy」タブから「gnss」を選択し「Inspector」タブを参照する

４．「Inspector」タブから「Add Component」ボタンを押下し「gnss」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-5 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-06.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブから「Add Component」ボタンを押下し「GNSS Sensor」を選択する

５.「GNSS Sensor」のコンポーネントが「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-6 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-07.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「GNSS Sensor」のコンポーネントが「Inspector」タブに追加されていることを確認する

６.再度「Inspector」タブから「Add Component」ボタンを押下し「Nav Sat Fix Msg Publisher」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-7 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-09-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 再度「Inspector」タブから「Add Component」ボタンを押下し「Nav Sat Fix Msg Publisher」を選択する

７.「Nav Sat Fix Msg Publisher」のコンポーネントが「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-8 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-09-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Nav Sat Fix Msg Publisher」のコンポーネントが「Inspector」タブに追加されていることを確認する

８.再度「Inspector」タブから「Add Component」ボタンを押下し「Geo Coordinate System」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-9 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-10-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 再度「Inspector」タブから「Add Component」ボタンを押下し「Geo Coordinate System」を選択する

９.「Geo Coordinate System」のコンポーネントが「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-10 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-10-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Geo Coordinate System」のコンポーネントが「Inspector」タブに追加されていることを確認する

10.「Inspector」タブを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-11 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-03-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブを確認する

11.「Inspector」タブを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-12 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-08.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブを確認する


12.unity のPlay ボタンを選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-13 
     - 操作
   * - .. image:: imu_gnss/img/unity-21.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity のPlay ボタンを選択する

13.「Inspector」タブが更新されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-14 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-10-3.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブに表示されている緯度、経度が現在地を示していることを確認する

「Inspector」タブの「Geo Coordinate System」コンポーネントの「Latitude、Longitude」が現在地を示していることを確認します

ROS Topic コマンドによるセンサモデルの設定情報取得とＩＭＵのデータ値設定
--------------------------------------------------------------------------

１．ROS環境の起動（zx120）

linux (ubuntu 18.04)環境を立ち上げる

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-1 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/ros-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linuxターミナルを立ち上げ　ROSCORE を起動する


２．実機で取得したROSBAG データを再生する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-2 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/ros-02.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linuxターミナルを立ち上げ 「rosbag play 2024-04-25-15-17-31.bag」を入力する

ショベルの実機通信サンプルデータ「2024-04-25-15-17-31.bag」をrosbag play で再生する

３．linuxターミナルを立ち上げ 「rostopic list」にてＩＭＵのトピック名称を確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-3 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/imu-a-7.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linuxターミナルを立ち上げ 「rosbag list」を入力する

例　boom の場合、「/zx120/boom/boom_imu」を確認する

４．実機で取得したサンプルデータから実際のIMU周期データを取得する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　4-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/imu-a-6.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linuxターミナルを立ち上げ 「rostopic hz /zx120/boom/boom_imu」を入力する

表示された周期から、平均的に１００hz を確認する

５．実機で取得したROSBAG データを再生からする/zx120/boom/boom_imu のセンサ情報の周期を「Inspector」タブにデータを設定する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-5 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/imu-a-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブで「Frequency」を入力する


５．IMUセンサの情報を「Inspector」タブにデータを設定する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-6 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/imu-a-2-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブで「Topic Name」と「Frame_id」を設定する


ＩＭＵセンサをショベルモデルに取り付けて位置調整する
--------------------------------------------------------------------------

１．ショベル実機のＩＭＵセンサをショベルモデルに取り付けて位置調整を行う

シミュレーション対応の実機についてＩＭＵセンサの取り付け位置を写真などにて確認する（例：zx120 boom_imu）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-1 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/IMG_2387.jpg
          :scale: 100%
          :height: 100px
          :width: 200px
     - 実機写真を参考に取り付け位置を確認する
   * - .. image:: imu_gnss/img/IMG_2394.jpg
          :scale: 100%
          :height: 100px
          :width: 200px
     - 実機写真を参考に取り付け位置を確認する
   * - .. image:: imu_gnss/img/imu-b-1-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editorで「Scene」タブを選択し「Ctrl」キーを押下しながら「マウス」を操作しショベルboomのimuの取り付け位置を調整する
   * - .. image:: imu_gnss/img/imu-b-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editorで「Scene」タブを選択し「Ctrl」キーを押下しながら「マウス」を操作しショベルboomのimuの取り付け位置を調整する
   * - .. image:: imu_gnss/img/imu-b-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editorで「Scene」タブを選択しショベルboomのimuの取り付け位置を確認

ＩＭＵセンサの取り付け位置でギズモのx-y-zの軸方向実機ショベルと一致するようにマウスで調整する（座標系の違い参照）

【参考】

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-2 　[拡大]
     - 説明
   * - .. image:: imu_gnss/img/unity-ros-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unityと実機ＩＭＵセンサでの座標系の違い
   * - .. image:: imu_gnss/img/unity-ros-02.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unityと実機ＩＭＵセンサでの座標系の変換方法


ＩＭＵセンサは、zx120ショベルの場合、swing、boom、arm、bucket　が存在する

２．IMUセンサの情報を「Inspector」タブデータを設定し確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-3 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/imu-b-3.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Unity Editorで「Hierarchy」タブから「zx120」「base_link」「body_link」「boom_link」を選択し「boom_imu」でx-y-z軸ギズモでimuオブジェクトの取り付け位置を確認する
   * - .. image:: imu_gnss/img/imu-b-3-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブデータを設定し確認する

同様の方法で、swing、arm、bucket、gnss について取り付け位置を調整する

