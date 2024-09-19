
センサモデルの追加方法
===============================

Unity Sensorsパッケージのインストール方法
------------------------------------------

１．ショベル実機のＩＭＵセンサの取り付け位置確認

シミュレーション対応の実機についてＩＭＵセンサの取り付け位置を
写真などにて確認する

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
   * - 　
     - "https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensors#v2.0.4"

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
   * - 　
     - "https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensorsROS#v2.0.4" 

９．UnitySensors パッケージがインストールされる

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-9 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-10.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensors パッケージがインストールされる

10．UnitySensors パッケージがインストールされたことを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　1-10 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-11.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - UnitySensors パッケージがインストールされたことを確認する

IMUセンサモデルの追加方法
--------------------------

１．Unityツールで空オブジェクトCreate Emptyの作成

Unityツール を起動し、ＩＭＵの空オブジェクトを作成する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　2-1 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity ツールを起動する
   * - .. image:: /imu_gnss/img/unity-01-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity メニューバーから「GameObject」「Create Empty」を選択する

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

４．「Inspector」タブから「Add Component」ボタンを押下しIMU Sensor」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-4 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-16.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブから「Add Component」ボタンを押下しIMU Sensor」を選択する

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

６.再度「Inspector」タブから「Add Component」ボタンを押下しIMU Msg Publisher 」を選択する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-6 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-18.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 再度「Inspector」タブから「Add Component」ボタンを押下しIMU Msg Publisher 」を選択する

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

10.「Inspector」タブが更新されていることを確認する

.. list-table::
   :widths: 15 10
   :header-rows: 1

   * - 図　2-10 　[拡大]
     - 操作
   * - .. image:: imu_gnss/img/unity-22.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Inspector」タブが更新されていることを確認する

GNSSセンサモデルの追加方法
--------------------------






