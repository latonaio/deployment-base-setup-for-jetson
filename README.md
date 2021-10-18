# deployment-base-setup-for-jetson  
deployment-base-setup-for-jetsonは、JetsonをセットアップするためのベースをPCでセットアップする手順概要です。

## 準備するもの

・UbuntuがインストールされたPC

## セットアップ手順

### Ubuntu上にNVIDIA SDK Managerをインストールする
Jetsonの開発環境について
こちらのダウンロードセンターに、NVIDIA SDK Managerのダウンロードリンクがあります。
[Jetson Download Center – NVIDIA Developer] (https://developer.nvidia.com/embedded/downloads)
上記からダウンロードしたdebパッケージをUbuntuへインストールします。

1.ubuntu上でterminalを立ち上げ、以下のコマンドを実行します。

```
 wget https://developer.nvidia.com/embedded/dlc/nv-sdk-manager

```
2.生成されたnv-sdk-managerファイルは、debパッケージとなっており、以下のコマンドでインストールできます。
```
 sudo dpkg -i ./nv-sdk-manager
```
3.  ライブラリが不足するケースがあるため、以下の操作を行います。以下コマンドで不足するライブラリをインストールします。

```
sudo apt install libgconf-2-4 libcanberra-gtk-module
```

4.  nv-sdk-managerをインストールします。

```
sudo dpkg -i ./nv-sdk-manager
```

### UbuntuデスクトップからSDK Managerを起動する。
以下の操作で、UbuntuデスクトップからSDK Managerを起動できるようになります。

1.	Ubuntu上でNVIDIA SDK Managerを起動する。
   1. GUI画面上でSDK Manager を起動します。画面左下の、点が9個（3×3）で並んでいるアプリボタンをタップすると各アプリを検索することができます。

   2. 検索窓から「SDK Manager」を検索することができます。
   
   3. 起動します。
   
  