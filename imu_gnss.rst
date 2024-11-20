
センサモデルの追加方法
===============================

Unity Sensorsパッケージのインストール方法
------------------------------------------

１．ショベル実機のＩＭＵセンサの取り付け位置確認

== =================================================================
　  シミュレーション対応の実機についてＩＭＵセンサの取り付け位置を

    写真などにて確認する（例：zx120）
== =================================================================

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

====== ==================================================================== ================================
　     【ＩＭＵセンサのシミュレーション確認手順概要】                        記載項目
１）   | 実機に取り付けられているＩＭＵセンサについてUnity Editor で         
       | シミュレーションする
２）    Unity Editor 内の UnitySensors パッケージをインストールする          ２．へ
３）   | それぞれのＩＭＵセンサについてUnity Editor 内のショベルモデルに     IMUセンサモデルの追加方法へ
       | Game Object を作成する
４）   | 実機ショベルで動作したＩＭＵセンサデータを取得して
       | 動作データを解析する
５）   | 実機ショベルで動作したデータを分析し、                             | センサモデルの設定情報取得と
       | シミュレーションに合致するように環境設定をする                     | ＩＭＵのデータ値設定
６）   | ROS - Unity Editor にてシミュレーションを実施してROS 側で
       | データを取得しシミュレーションが正しく動作していることを確認する
====== ==================================================================== ================================


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
     
３．  Package Manager ウィンドウのメニューバーから「＋」「Add package from git URL」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-3 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-03.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Manager ウィンドウの例
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
     - Package Manager ウィンドウのＵＲＬ入力テキストボックスに

       下記のURLを入力し「Add」ボタンを押下する
   * - 入力するURL【※１】
     - https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensors#v2.0.4"

===================== =======================================================================
 【※１注意】          | Package のバージョンについては、
                      | 記載時以降にバージョンアップされる場合があります
                      | 下記のURL にて最新バージョンを確認の上
                      | 対応のPackage についてURLを入力してください
 Assets/UnitySensors    https://github.com/Field-Robotics-Japan/UnitySensors
===================== =======================================================================

５．UnitySensors パッケージがインストールされることを確認する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　1-5 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-07.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensors パッケージがインストールされる

６．UnitySensors パッケージが図の内容のようにインストールされたことを確認する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　1-6 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-08.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensors パッケージがインストールされたことを確認する

７．UnitySensorsROS パッケージのインストール

Package Manager ウィンドウのメニューバーから再度、「＋」「Add package from git URL」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-7　[拡大] 
     - 操作
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
     - Package Manager ウィンドウのＵＲＬ入力テキストボックスに

       下記のURLを入力し「Add」ボタンを押下する
   * - 入力するURL【※２】
     - https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensorsROS#v2.0.4 

===================== =======================================================================
【※２】注意           | Package のバージョンについては、
                      | 記載時以降にバージョンアップされる場合があります
                      | 下記のURL にて最新バージョンを確認の上
                      | 対応のPackage についてURLを入力してください
 Assets/UnitySensors   https://github.com/Field-Robotics-Japan/UnitySensors
===================== =======================================================================

９．UnitySensorsROS パッケージがインストールされる

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　1-9 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-10.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensorsROS パッケージがインストールされることを確認する

10．UnitySensorsROS パッケージが図の内容のようにインストールされたことを確認する

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
     - Unity Editorを起動する
   * - .. image:: /imu_gnss/img/unity-01-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity 「Hierarchy」タブから「zx120」「base_link」「body_link」「boom_link」

       を選択し右クリックで「Create Empty」を選択する

=== ===========================================================
　  | boom_imu の場合、ショベルの実機写真（図　1-1 ）から
    | ショベルモデルのboom_link から空オブジェクトを作成する
=== ===========================================================

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
     - unity 「Hierarchy」タブから「boom_imu」を選択し

       「Inspector」タブを参照する

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
     - 「Inspector」タブから「Add Component」ボタンを押下し

        「IMU Sensor」を選択する

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
     - 「IMU Sensor」のコンポーネントが「Inspector」タブに

         追加されていることを確認する

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
     - 再度「Inspector」タブから「Add Component」ボタンを押下し

       「IMU Msg Publisher 」を選択する

７.「IMU Msg Publisher」のコンポーネントが図のように「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-7 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-19.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「IMU Msg Publisher」のコンポーネントが「Inspector」タブに

         追加されていることを確認する

８.「Inspector」タブを確認する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　2-8 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-20.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブの追加コンポーネントを確認する

９.unity のPlay ボタンを選択する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　2-9 
     - 操作
   * - .. image:: imu_gnss/img/unity-21.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity EditorのPlay 「▶」ボタンを選択する

10.「Inspector」タブが図のようにデータ更新されていることを確認する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　2-10 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-22.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブがデータ更新されていることを確認する

=== ================================================
　  | 同様の方法で、swing、arm、bucket について
    | ＩＭＵセンサモデルを追加する
=== ================================================

GNSSセンサモデルの追加方法
--------------------------

１．ショベル実機のＧＮＳＳセンサの取り付け位置確認

=== ====================================================================
　  | シミュレーション対応の実機についてＧＮＳＳセンサの取り付け位置を
    | 写真などにて確認する（例：zx120）
=== ====================================================================

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

=== ====================================================================
　  | ＧＮＳＳセンサは、実機写真からショベルモデルの　body部分に
    | 設定されていることを確認する 
=== ====================================================================


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
     - Unity Editor を起動する
   * - .. image:: /imu_gnss/img/gnss-02.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor 「Hierarchy」タブから「zx120」「base_link」「body_link」

       を選択し右クリックで「Create Empty」を選択する

３．「Inspector」タブで GameObjectに名称を設定する（例：gnss）

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


３．Unity Editor 「Hierarchy」タブから「gnss」を選択し「Inspector」タブを参照する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-05.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor 「Hierarchy」タブから「gnss」を選択し

       「Inspector」タブを参照する

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
     - 「Inspector」タブから「Add Component」ボタンを押下し

       「GNSS Sensor」を選択する

５.「GNSS Sensor」のコンポーネントが図のように「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-6 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-07.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「GNSS Sensor」のコンポーネントが「Inspector」タブに

         追加されていることを確認する

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
     - 再度「Inspector」タブから「Add Component」ボタンを押下し

       「Nav Sat Fix Msg Publisher」を選択する

７.「Nav Sat Fix Msg Publisher」のコンポーネントが図のように「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　3-8 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-09-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Nav Sat Fix Msg Publisher」のコンポーネントが

        「Inspector」タブに追加されていることを確認する


８.Unity Editor のPlay ボタンを選択する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　3-9 
     - 操作
   * - .. image:: imu_gnss/img/unity-21.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor のPlay 「▶」ボタンを選択する

９.「ショベルモデル」を駆動してシミュレーションにて緯度、経度が更新されていることを確認する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　3-10 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/gnss-11-3-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor でショベルモデルを動作させる（動作前）
   * - .. image:: imu_gnss/img/gnss-11-2-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Unity Editor でショベルモデルを動作させる（動作後）

         を示していることを確認する
   * - .. image:: imu_gnss/img/gnss-11-1-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「ROS」にてtopic echo で表示されている緯度、経度が

         変更していることを確認する

=== ==================================================================
　   「Inspector」タブの「Geo Coordinate System」コンポーネントの

     「Latitude、Longitude」が作業を実施する原点位置を

      示していることを確認する
=== ==================================================================



GPSの座標を Unity Editor の地形データに割り付ける（地形の原点座標となる）
--------------------------------------------------------------------------

１．Unity Editor の「Hierarchy」タブから「Terrain」を選択し「Inspector」タブを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　4-1 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/terrain-01-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Hierarchy」タブから「Terrain」を選択し「Inspector」タブを確認する



２．Unity Editorで空オブジェクトCreate Emptyを作成する

Unity Editor を起動し、「Terrain」を選択し空オブジェクトを作成する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-2 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/terrain-02-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor 「Hierarchy」タブから「Terrain」を選択し

        右クリックで「Create Empty」を選択する


３．「Inspector」タブで GameObjectに名称を設定する（例：GeoCoordinateSystem）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-3 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/terrain-03-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - GameObjectに名称を設定する（例：GeoCoordinateSystem）


４．Unity Editor 「Hierarchy」タブから「Terrain」を選択し「Inspector」タブの「GeoCoordinateSystem」を参照する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　4-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/terrain-03-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor 「Hierarchy」タブから「Terrain」を選択し

       「Inspector」タブの「GeoCoordinateSystem」を参照する

５．「Inspector」タブから「Add Component」ボタンを押下し「Geo Coordinate System」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　4-5 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/terrain-04-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブから「Add Component」ボタンを押下し

        「Geo Coordinate System」を選択する

６.「Geo Coordinate System」のコンポーネントが「Inspector」タブに追加されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　4-6 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/terrain-05-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Geo Coordinate System」のコンポーネントが

        「Inspector」タブに追加されていることを確認する


センサモデルの設定情報取得とＩＭＵのデータ値設定
--------------------------------------------------------------------------

１．ROS環境の起動（zx120）

　　　例：linux (ubuntu 18.04)環境を立ち上げる

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-1 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/ros-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linuxターミナルを立ち上げ　ROSCORE を起動する
   * - 入力するコマンド
     - roscore


２．ROS-Unity 間通信環境を立ち上げる

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-2 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/ros-unity-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 別のlinuxターミナルを立ち上げ 

       「roslaunch ros_tcp_endpoint endpoint.launch」を入力する
   * - 入力するコマンド
     - roslaunch ros_tcp_endpoint endpoint.launch


３．linuxターミナルを立ち上げ 「rostopic list」にてＩＭＵのトピック名称を確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-3 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/imu-a-7.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linuxターミナルを立ち上げ 「rostopic list」を入力する
   * - 入力するコマンド
     - rostopic list

　　　表示されたrostopic のリストから、

　　　例　boom の場合、「/zx120/boom/g2_imu」を確認する

４．実機で取得したサンプルデータから実際のIMU周期データを取得する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　5-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/imu-a-6.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linuxターミナルを立ち上げ 「rostopic hz /zx120/boom/g2_imu」を入力する
   * - 入力するコマンド
     - rostopic hz /zx120/boom/g2_imu

画面に表示された周期から、平均的に１００hz を確認する

５．取得した通信データから　/zx120/boom/g2_imu のセンサ情報の周期を「Inspector」タブにデータを設定する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-5 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/imu-a-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブで「Frequency」を入力する　２か所


６．IMUセンサの情報を「Inspector」タブに実機に合わせるため通信名称のデータを設定する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-6 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/imu-a-2-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブで「Topic Name」と「Frame_id」

         に実機と同じ通信名称を設定する

７．Unity Editor ショベルモデルで作成したＩＭＵセンサについてシミュレーションを実施する

　Unity Editor ショベルモデルで作成したＩＭＵセンサについてシミュレーションを実施して

　ＩＭＵセンサのシミュレーション動作を確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-7 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/unity-ros-03-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity-ros のシミュレーション環境の確認
   * - 　
     - linux Terminal を２画面立ち上げる「roscore」と

       「roslaunch ros_tcp_endpoint endpoint.launch」

８.Unity Editorを立ち上げ　Play ボタンを選択する

.. list-table::
   :widths: 10 15
   :header-rows: 1

   * - 図　5-8 
     - 操作
   * - .. image:: imu_gnss/img/unity-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor を立ち上げる
   * - .. image:: imu_gnss/img/unity-21.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editor のPlay 「▶」ボタンを選択する

９．unity-ros 通信によるショベルモデルのシミュレーション状態を確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-9 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/unity-ros-04.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity-ros 通信によるショベルモデルのシミュレーション

10．ショベルモデルのシミュレーション動作確認

　　例：ＩＭＵセンサのboom部、トピック名「/zx120/boom/g2_imu」

　　について通信内容をモニタリングして確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-10 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/imu-a-7.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linux Terminal を起動して「rostopic list」を入力する
   * - 入力コマンド
     - rostopic list

11．IMUセンサの情報を「Inspector」タブに実機に合わせるため通信名称のデータを設定する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-11 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/unity-ros-06-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - linux Terminal を起動して「/zx120/boom/g2_imu」を

        入力してシミュレーション動作を確認する
   * - 入力コマンド
     - rostopic echo /zx120/boom/g2_imu
   * - .. image:: imu_gnss/img/imu-a-2-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブで「Topic Name」と「Frame_id」

         に実機と同じ通信名称を設定する

12．シミュレーション動作の結果を確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-13 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/unity-ros-06-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - frame_id　の表示を図のようになっているかを確認する
   * - .. image:: imu_gnss/img/unity-ros-06-3.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - ＩＭＵセンサのシミュレーション結果のデータを確認する
   * - orientation:
     - ＩＭＵセンサの結果の座標データx-y-x-wデータを確認する
   * - angular_velocity:
     - ＩＭＵセンサの結果の角速度x-y-zデータを確認する
   * - linear_acceleration:
     - ＩＭＵセンサの結果の角加速度x-y-zデータを確認する

=== ============================================================================
　   シミュレーション結果のデータについて実機ＩＭＵセンサのデータと比較して

     問題がないかどうかを検討する

     また、同様の方法で、swing、arm、bucket について

     シミュレーション結果のデータについて実機ＩＭＵセンサのデータと比較して

     問題がないかどうかを検討する
=== ============================================================================


Unity Editor ショベルモデルの scene 空間でＩＭＵセンサを取り付けて位置情報と座標軸を調整する
----------------------------------------------------------------------------------------------------------------

１．ショベル実機のＩＭＵセンサと同じ位置にショベルモデルに取り付けて位置調整を行う

　　　シミュレーション対応の実機についてＩＭＵセンサの取り付け位置を

　　　写真などにて確認する（例：zx120 boom_imu）

　　　ショベルモデルと実機が完全に一致しない場合、近い位置に設置する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　6-1 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/zx120-01.jpg
          :scale: 100%
          :height: 100px
          :width: 100px
     - 実機写真を参考に取り付け位置を確認する#1
   * -  .. image:: imu_gnss/img/zx120-04.jpg
          :scale: 100%
          :height: 100px
          :width: 100px
     - 実機写真を参考に取り付け位置を確認する#2
   * - .. image:: imu_gnss/img/imu-b-1-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editorで「Scene」タブを選択し「Ctrl」キーを押下しながら

       「マウス」を操作しショベルboomのimuの取り付け位置を選択する
   * - .. image:: imu_gnss/img/imu-b-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 選択したboom のimu の取り付け位置を確認する

　　　ＩＭＵセンサの取り付け位置でギズモのx-y-zの軸方向実機ショベルと

　　　一致するようにマウスで調整する（座標系の違い参照）

【参考】

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　6-2 　[拡大]
     - 説明
   * - .. image:: imu_gnss/img/zahyo-01.jpg
          :scale: 100%
          :height: 100px
          :width: 100px
       .. image:: imu_gnss/img/zahyo-02.jpg
          :scale: 100%
          :height: 100px
          :width: 100px
     - unityと実機(ROS)ＩＭＵセンサでの座標系の違い
   * - .. image:: imu_gnss/img/zahyo-05.jpg
          :scale: 100%
          :height: 100px
          :width: 100px
     - unityと実機(ROS)ＩＭＵセンサでの座標系の変換方法


ＩＭＵセンサは、zx120ショベルの場合、swing、boom、arm、bucket　が存在する

２．IMUセンサの情報を「Inspector」タブデータを設定し確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　6-3 　[拡大]
     - 内容
   * - .. image:: imu_gnss/img/imu-b-3.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Unity Editorで「Hierarchy」タブから「zx120」「base_link」

       「body_link」「boom_link」を選択し「boom_imu」でx-y-z軸ギズモで

       imuオブジェクトの取り付け位置を確認する
   * - .. image:: imu_gnss/img/imu-b-3-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブデータを設定し確認する

同様の方法で、swing、arm、bucket、gnss について取り付け位置を調整する

