
##########################
IMUとGNSSの取り付け方法
##########################

IMUとGNSSの取り付け方法の詳細
===============================


１．ショベル実機のＩＭＵセンサの取り付け位置確認
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/IMG_2394.jpg
   :scale: 100%
   :height: 100px
   :width: 200px



２．Create Emptyの作成
^^^^^^^^^^^^^^^^^^^^^^^^

  unity メニューバーから「GameObject」「Create Empty」を選択する

.. image:: ./img/unity-01.png
   :scale: 100%
   :height: 100px
   :width: 200px

３．GameObjectに名称を設定する（例：boom_imu）
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-02-1.png
   :scale: 100%
   :height: 100px
   :width: 200px


４．UnitySensors パッケージのインストール
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  unity メニューバーから「Windows」「Package Manager」を選択する

.. image:: ./img/unity-02.png
   :scale: 100%
   :height: 100px
   :width: 200px


５．Package Manager ウィンドウのメニューバーから「＋」「Add package from git URL」を選択する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-03.png
   :scale: 100%
   :height: 100px
   :width: 200px

.. image:: ./img/unity-04.png
   :scale: 100%
   :height: 100px
   :width: 200px


６．Package Manager ウィンドウのＵＲＬ入力テキストボックスに下記のURLを入力し「Add」ボタンを押下する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   「https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensors#v2.0.4」

.. image:: ./img/unity-06.png
   :scale: 100%
   :height: 100px
   :width: 200px

７．UnitySensors パッケージがインストールされる
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-07.png
   :scale: 100%
   :height: 100px
   :width: 200px

８．UnitySensors パッケージがインストールされたことを確認する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-08.png
   :scale: 100%
   :height: 100px
   :width: 200px


７．Package Manager ウィンドウのメニューバーから再度、「＋」「Add package from git URL」を選択する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-03.png
   :scale: 100%
   :height: 100px
   :width: 200px

.. image:: ./img/unity-04.png
   :scale: 100%
   :height: 100px
   :width: 200px


８．Package Manager ウィンドウのＵＲＬ入力テキストボックスに下記のURLを入力し「Add」ボタンを押下する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   「https://github.com/Field-Robotics-Japan/UnitySensors.git?path=/Assets/UnitySensorsROS#v2.0.4」

.. image:: ./img/unity-09.png
   :scale: 100%
   :height: 100px
   :width: 200px

９．UnitySensors パッケージがインストールされる
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-10.png
   :scale: 100%
   :height: 100px
   :width: 200px

１０．UnitySensors パッケージがインストールされたことを確認する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-11.png
   :scale: 100%
   :height: 100px
   :width: 200px


１１．unity 「Hierarchy」タブから「boom_imu」を選択し「Inspector」タブを参照する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-15.png
   :scale: 100%
   :height: 100px
   :width: 200px


１２．「Inspector」タブから「Add Component」ボタンを押下しIMU Sensor」を選択する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-16.png
   :scale: 100%
   :height: 100px
   :width: 200px


１３．「IMU Sensor」のコンポーネントが「Inspector」タブに追加されていることを確認する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-17.png
   :scale: 100%
   :height: 100px
   :width: 200px


１４．再度「Inspector」タブから「Add Component」ボタンを押下しIMU Msg Publisher 」を選択する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-18.png
   :scale: 100%
   :height: 100px
   :width: 200px


１５．「IMU Msg Publisher」のコンポーネントが「Inspector」タブに追加されていることを確認する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-19.png
   :scale: 100%
   :height: 100px
   :width: 200px


１６．「Inspector」タブを確認する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-20.png
   :scale: 100%
   :height: 100px
   :width: 200px



１７．unity のPlay ボタンを選択する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-21.png
   :scale: 100%
   :height: 100px
   :width: 200px



１８．「Inspector」タブが更新されていることを確認する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ./img/unity-22.png
   :scale: 100%
   :height: 100px
   :width: 200px



