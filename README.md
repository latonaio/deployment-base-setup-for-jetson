# JetsonをセットアップするためのベースをPCでセットアップする手順

## 準備

- UbuntuがインストールされたPC

## セットアップ手順

### Ubuntu上にNVIDIA SDK Managerをインストール
Jetsonの開発環境について

こちらのダウンロードセンターに、NVIDIA SDK Managerのダウンロードリンクがあります。
[Jetson Download Center – NVIDIA Developer] (https://developer.nvidia.com/embedded/downloads)
上記からダウンロードしたdebパッケージをUbuntuへインストールします。

1. ubuntu上でterminalを立ち上げ、以下のコマンドを実行します。

```
 wget https://developer.nvidia.com/embedded/dlc/nv-sdk-manager

```
2. 生成されたnv-sdk-managerファイルは、debパッケージとなっており、以下のコマンドでインストールできます。
```
 sudo dpkg -i ./nv-sdk-manager
```
3.  不足しているライブラリをインストールします。

```
sudo apt install libgconf-2-4 libcanberra-gtk-module
```

4.  nv-sdk-managerをインストールします。

```
sudo dpkg -i ./nv-sdk-manager
```

### UbuntuデスクトップからSDK Managerを起動

1.	Ubuntu上でNVIDIA SDK Managerを起動する。

2. GUI画面上でSDK Manager を起動します。画面左下の、点が9個（3×3）で並んでいるアプリボタンをタップすると各アプリを検索することができます。

3. 検索窓から「SDK Manager」を検索することができます。
   
4. 起動します。
   
  