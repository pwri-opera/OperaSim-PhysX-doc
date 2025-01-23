
建機モデルの追加方法
===============================

既存重機モデルを追加する方法
------------------------------------------

【サンプルモデルの例：zx120ショベルの場合】

| =============================================
| １．ショベル実機の既存３Ｄモデルデータから 
|      unity editor にモデルを追加する方法
| =============================================

１－１．既存の３Ｄモデルデータのエクスポート（Prefab の作成）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-1 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | unity editor から既存のショベルモデルを選択する
       | 例：zx120ショベル

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-2 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-02.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Prefab」「GameObject」「Export To FBX」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-3 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-03.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Export Option」ウインドウが表示される

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-4 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-04.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Export」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-5 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-04-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Export されたFBXファイルをエクスプローラで確認する


１－２．既存の３Ｄモデルデータを同一プロジェクトへのインポートする（Prefab）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-6 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-12.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Project」「Assets」「Prefab」参照タブ右クリック「Convert TO FBX Prefab Variant...」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-7 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-13.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Project」「Assets」「Prefab」内の既存ショベルモデル「zx120.fbx」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-8 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-14.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「zx120」を選択し「Hierarchy」タブにドラッグ＆ドロップする

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-9　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-16.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 生成された既存の３Ｄモデルを確認する

※インポートした新規ショベルモデルの動作用初期設定については別途記載

１－３．既存の３Ｄモデルデータを別プロジェクトへのインポートする（Prefab）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-10 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-05.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - エクスポートした既存ショベルモデルをインポートする

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-11 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-06.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Assets」「Import New Assets」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-12 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-08.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - エクスポートした既存ショベルモデル「zx120.fbx」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-13 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-11.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - インポートした既存ショベルモデルを確認する

※インポートした新規ショベルモデルの動作用初期設定については別途記載


新規重機モデルの作成方法
------------------------------------------


油圧ショベル
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

【サンプルモデル 例：zx120ショベルの場合】

| ======================================================
| １．ショベル実機の３Ｄモデルデータ(URDF)から
|      unity editor に新規ショベルモデルを追加する方法
| ======================================================

１－１．URDF Importer のパッケージ追加

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-14 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-17.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity editor から「Window」「Package Manager」を選択する


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-15 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-18.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | 「Package Manager」ウインドウから「+」
       | 「Add package from git URL...」を選択する


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-16 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-19.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | 「Package Manager」ウインドウから「下記のURL」を入力し
       | 「Add」を選択する

========= =========================================================================================================
  ＵＲＬ    https://github.com/Unity-Technologies/URDF-Importer.git?path=/com.unity.robotics.urdf-importer#v0.5.2
========= =========================================================================================================

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-17 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-21.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - URDF Importer のパッケージがインストールされる

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-18 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-22.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - URDF Importer のパッケージのインストールを確認する

インポートする新規の重機モデル(urdf)ファイルをunity editor 内にコピーする

+-------+----------------------------------------------------+
+ urdf  + 例：roid1_urdf_unuty.urdf　ファイル                +
+-------+----------------------------------------------------+

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-19 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-23.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | 「Project」タブから「Assets」「３DモデルのURDFデータ」を選択し
       | 右クリックで「Import Robot from Selected URDF file」を選択する


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-20 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-24.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | 「URDF import Setting」タブから『Y Axiss』『VHACD』を選択し
       | 「Import URDF」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-21 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-26.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 新規ショベルモデルが追加されたことを確認する


１－２．追加したショベルモデルの動作用初期設定

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-22 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-01.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - unity editorを確認する

１－２－１）Package Manager　：　In Project の追加初期設定

+---------------------------------------------------------------------------------------------------------------------------+
| 「Package Manager」の設定で「Packages In Project」 を選択し                                                               |
+---------------------------------------------------------------------------------------------------------------------------+
| 下図に示す「Package - Unity」のリストで不足しているライブラリを選択してインストールする                                   |
+---------------------------------------------------------------------------------------------------------------------------+
| 「更新前」から「更新後」のように追加インストールする                                                                      |
+---------------------------------------------------------------------------------------------------------------------------+


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-23 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-04.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | 「Window」「Package Manager」In Project の追加初期設定として
       |  更新前から更新後までを実施する

ライブラリーの更新手順（繰り返し実施する）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-24 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-02.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Window」「Package Manager」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-25 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-03-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Managerタブの「Packages:」「▼」を選択し「In-Project」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-26 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-04-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Managerタブのライブラリー一覧を確認する


+----------------------------------------------------------------------------------+
| ライブラリー一覧から下記の一覧で未インストールのライブラリーがあれば             |
+----------------------------------------------------------------------------------+
| 「+」「Add package from git URL...」を選択する                                   |
+----------------------------------------------------------------------------------+
| 下記の表から指定のURL をコピーしてテキストボックスにURL を貼り付けて             |
+----------------------------------------------------------------------------------+
| 所定のライブラリーをインストールする                                             |
+----------------------------------------------------------------------------------+


追加でインストールするライブラリー一覧

+-------------+---------------------------------------------------------------------------------------------------------------------------+----------+
| 種別名称    | インストールするライブラリ名称                                                                                            | チェック |
+             +---------------------------------------------------------------------------------------------------------------------------+----------+
| ＵＲＬ      | インストールするライブラリＵＲＬ                                                                                          |          |
+-------------+---------------------------------------------------------------------------------------------------------------------------+----------+
| 13Pixels    | GitMerge for Unity                                                                                                        |          |
+             +---------------------------------------------------------------------------------------------------------------------------+----------+
|             | https://github.com/FlaShG/GitMerge-for-Unity.git                                                                          |          |
+-------------+---------------------------------------------------------------------------------------------------------------------------+----------+
| Other       | Jobs                                                                                                                      |          |
+             +---------------------------------------------------------------------------------------------------------------------------+----------+
|             | https://github.com/needle-mirror/com.unity.jobs.git                                                                       |          |
+-------------+---------------------------------------------------------------------------------------------------------------------------+----------+
| Other       | ROS TCP Connector                                                                                                         |          |
+             +---------------------------------------------------------------------------------------------------------------------------+----------+
|             | https://github.com/Unity-Technologies/ROS-TCP-Connector.git?path=/com.unity.robotics.ros-tcp-connector#v0.7.1             |          |
+-------------+---------------------------------------------------------------------------------------------------------------------------+----------+
| Other       | Unity Robotics Visualizations                                                                                             |          |
+             +---------------------------------------------------------------------------------------------------------------------------+----------+
|             | https://github.com/Unity-Technologies/ROS-TCP-Connector.git?path=/com.unity.robotics.visualization                        |          |
+-------------+---------------------------------------------------------------------------------------------------------------------------+----------+
| Other       | URDF Importer                                                                                                             |          |
+             +---------------------------------------------------------------------------------------------------------------------------+----------+
|             | https://github.com/Unity-Technologies/URDF-Importer.git?path=/com.unity.robotics.urdf-importer#v0.                        |          |
+-------------+---------------------------------------------------------------------------------------------------------------------------+----------+

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-27 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-04.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Managerタブのライブラリー一覧を確認する



１－２－２）Package Manager　：　Unity Registry の追加初期設定

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-28 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-05.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Managerタブのライブラリー一覧を確認する

+-------------------------------------------------------------------------------------------+
| 「Package Manager」の設定で「Packages Unity Registry」 を選択し                           |
+-------------------------------------------------------------------------------------------+
| 下図に示す「Package - Unity」のリストで不足しているライブラリを選択してインストールする   |
+-------------------------------------------------------------------------------------------+
| 「更新前」から「更新後」のように追加インストールする                                      |
+-------------------------------------------------------------------------------------------+

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-29 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-05-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Managerタブの「Packages:」「▼」を選択し「Unity Registry」を選択する

+-------------+---------------------------------------------------------------+----------+
| 種別名称    | インストールするライブラリ名称                                | チェック |
+             +---------------------------------------------------------------+----------+
| ＵＲＬ      | インストールするライブラリＵＲＬ                              |          |
+-------------+---------------------------------------------------------------+----------+
| Unity       | AI Navigation                                                 |          |
+             +---------------------------------------------------------------+----------+
|             | FBX Exporter                                                  |          |
+             +---------------------------------------------------------------+----------+
|             | Unity Profiling Core API                                      |          |
+-------------+---------------------------------------------------------------+----------+
| Unity       | Autodesk FBX SDK for Unity                                    |          |
+             +---------------------------------------------------------------+----------+
|             | https://github.com/Unity-Technologies/com.autodesk.fbx.git    |          |
+-------------+---------------------------------------------------------------+----------+

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-30 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-13-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | Package Managerタブの「Packages」からインストールする
       | 「AI Navigation」を選択し右上の「Install」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-31 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-13-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「AI Navigation」がインストールされる

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-32 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-13-3.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「AI Navigation」のインストールを確認する

不足しているライブラリを選択してインストールする 

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　1-33 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-05-3.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - Package Managerタブのライブラリー一覧を確認する


２）作成済Script の追加初期設定

作成済のScript をシミュレーションモデルにアサインする


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　2-1 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-08-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Project」「Assets」「Create」「Folder」を選択し「Script」を入力しフォルダーを作成する

+-------------+----------------------------------------+
| データ種別  | Script 一覧                            |
+-------------+----------------------------------------+
| Folder      | BAPointCloudRenderer                   |
+-------------+----------------------------------------+
| Folder      | Editor                                 |
+-------------+----------------------------------------+
| File        | BucketRocks.cs                         |
+-------------+----------------------------------------+
| Files       | Clock.cs                               |
+-------------+----------------------------------------+
| Files       | ConvexHullCalculator.cs                |
+-------------+----------------------------------------+
| Files       | CustomCollisionIZX120.cs               |
+-------------+----------------------------------------+
| Files       | FollowJointTrajectoryAction.cs         |
+-------------+----------------------------------------+
| Files       | GroundTruthPublisher.cs                |
+-------------+----------------------------------------+
| Files       | GroundTruthTFPublisher.cs              |
+-------------+----------------------------------------+
| Files       | JointPosController.cs                  |
+-------------+----------------------------------------+
| Files       | JointStatePublisher.cs                 |
+-------------+----------------------------------------+
| Files       | NewLayer 1.terrainlayer                |
+-------------+----------------------------------------+
| Files       | NewLayer.terrainlayer                  |
+-------------+----------------------------------------+
| Files       | OdomPublisher.cs                       |
+-------------+----------------------------------------+
| Files       | OperaSimPhysXAssembly.asmdef           |
+-------------+----------------------------------------+
| Files       | PoseStampedPublisher.cs                |
+-------------+----------------------------------------+
| Files       | QuaternionStampedPublisher.cs          |
+-------------+----------------------------------------+
| Files       | RealtimeFactorProfiler.cs              |
+-------------+----------------------------------------+
| Files       | ROSClockPublisher.cs                   |
+-------------+----------------------------------------+
| Files       | SoilParticleSettings.cs                |
+-------------+----------------------------------------+
| Files       | TimeStamp.cs                           |
+-------------+----------------------------------------+
| Files       | VesselController.cs                    |
+-------------+----------------------------------------+


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　2-2　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-11.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Scripts」フォルダーに作成済のスクリプトデータをコピーする

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　2-3 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-09-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Scripts」フォルダーに作成済のスクリプトデータを確認する

３）ショベルモデルのinspector データ初期設定

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-1　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-20.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - | unity editeorの「Hierarchy」 で追加したショベルモデルの
       | 各関節をツリー表示する
       | zx120、base_link、body_link、boom_link、arm_link、bucket_link など


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-2 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-01-0-zx120.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - zx120のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-3 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-02-base-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - base_linkのInspectorを確認する


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-4 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-03-0-body.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - body_linkのInspectorを確認する


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-5 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-04-boom-1-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - boom_linkのInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-6 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_param-24.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - arm_linkのInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-7 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-05-arm-1-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - bucket_linkのInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-8 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-06-bucket-1-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - bucket_linkのInspectorを確認する


+-------------------------------------------------------------------------------+
+ 駆動関節部分のInspector Component　が不足しているcomponent　について          +
+-------------------------------------------------------------------------------+
+ 「Add Component」ボタンを選択して追加し                                       +
+-------------------------------------------------------------------------------+
+ component が追加されていることを確認する                                      +
+-------------------------------------------------------------------------------+

+-------------+------------------+---------+---------------------------+
|             | Game Object Name |  Active | Component                 |
+-------------+------------------+---------+---------------------------+
| Inspector   | zx120            |   〇    | Transform                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Robot                |
+             +                  +---------+---------------------------+
|             |                  |         | Controller                |
+             +                  +---------+---------------------------+
|             |                  |         | Rigidbody                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Box Collidar              |
+             +                  +---------+---------------------------+
|             |                  |         | Fixed Joint               |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Joint State Publisher     |
+-------------+------------------+---------+---------------------------+
| Inspector   | base_link        |   〇    | Transform                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Articulation body         |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Inertial             |
+-------------+------------------+---------+---------------------------+
|Inspector    | body_link        |   〇    | Transform                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Articulation body         |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Inertial             |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Joint Continuous     |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Joint Pos Controller      |
+             +                  +---------+---------------------------+
|             |                  |         | Pose Stamped Publisher    |
+-------------+------------------+---------+---------------------------+
|Inspector    | boom_link        |   〇    | Transform                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Articulation body         |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Inertial             |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Joint Revolute       |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Joint Pos Controller      |
+-------------+------------------+---------+---------------------------+
|Inspector    | arm_link         |   〇    | Transform                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf link                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Articulation body         |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Inertial             |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Joint Revolute       |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Joint Pos Controller      |
+-------------+------------------+---------+---------------------------+
|Inspector    | bucket_link      |   〇    | Transform                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf link                 |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Articulation body         |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Inertial             |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Urdf Joint Revolute       |
+             +                  +---------+---------------------------+
|             |                  |   〇    | Joint Pos Controller      |
+-------------+------------------+---------+---------------------------+

Inspector の追加方法（例：boom_link）

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-9 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-010-boom-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - boom関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-10 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-010-boom-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - boom関節部のInspectorで「Add Component」を選択する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-11 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-010-boom-3.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Joint Pos Controller」を入力しComponentを追加する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　3-12 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-010-boom-4.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - 「Joint Pos Controller」のInspectorを確認する




４）ショベルモデルの初期設定データの初期作成


４－１）zx120

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-1 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-01-zx120.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - zx120関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-2 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-01-0-zx120.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - zx120関節部のInspectorを確認する

４－２）base_link

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-3 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-02-base.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - base_link 関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-4 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-02-base-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - base_link 関節部のInspectorを確認する

４－３）body_link

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-5 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-03-body.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - base_link 関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-6 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-03-0-body.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - base_link 関節部のInspectorを確認する

４－４）boom_link


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-7 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-04-boom-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - boom_link 関節部のInspectorを確認する


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-8 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-04-boom-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - boom_link 関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-9 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-04-boom-1-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - boom_link 関節部のInspectorを確認する

４－５）arm_link


.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-10 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-05-arm-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - arm_link 関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-11 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-05-arm-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - arm_link 関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-12 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-05-arm-1-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - arm_link 関節部のInspectorを確認する

４－６）bucket_link

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-13 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-06-bucket-1.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - bucket_link 関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-14 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-06-bucket-2.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - bucket_link 関節部のInspectorを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　4-15 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/initial_inspector-06-bucket-1-0.png
          :scale: 100%
          :height: 100px
          :width: 200px
     - bucket_link 関節部のInspectorを確認する

５)追加したショベルモデルの関節部の駆動動作テスト

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-1 　[拡大]
     - 内容
   * - .. image:: construction_machine_model/img/prefab-01.gif
          :scale: 100%
          :height: 100px
          :width: 200px
     - 追加された新規ショベルモデルが動作することを確認する

.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - 図　5-2 　[拡大]
     - 内容
   * - .. figure:: construction_machine_model/img/unityショベル-02-1.mp4
          :class: controls
          :scale: 100%
          :height: 100px
          :width: 200px
     - 追加された新規ショベルモデルが動作することを確認する
   * - .. figure:: construction_machine_model/img/unityショベル-03-1.mp4
          :class: controls
          :scale: 100%
          :height: 100px
          :width: 200px
     - 追加された新規ショベルモデルが動作することを確認する


クローラダンプ
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ブルドーザ
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

