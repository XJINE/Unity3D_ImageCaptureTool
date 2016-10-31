# Unity3D_ImageCaptureTool

Unity3D で指定したカメラの画像をキャプチャするためのツールです。スクリーンショットを撮影したり、背景が透過なテクスチャ素材を生成するときなどに利用します。

## 導入・仕様方法

任意のプロジェクトの Assets ディレクトリに ./Editor/ImageCaptureTool.cs を追加すると、ツールバーに ./Custom/ImageCaptureTool が追加されます。
ImageCaptureTool のウィンドウを開いて、クリックかキー入力によって画像をキャプチャすることができます。

## 主な機能

- 任意の出力先とファイル名を指定することができます。
- 任意のカメラを指定してキャプチャすることができます。
- 画像は透過度付き(アルファチャネルを含むARGB32)で出力されます。
- 解像度は次の2種類を指定することができます。
    - 完全に任意に指定する解像度 * 任意の拡大率の解像度。
    - GameView の解像度 * 任意の拡大率の解像度。
- カメラの設定にかかわらず背景を透過して撮影する機能があります。
- 複数のカメラを登録して、同時に撮影することができます。
    - カメラごとに解像度を指定することができます。
    - カメラごとにSuffixを指定することができます。
    
## 仕様

### 出力パスについて

現在のところ無効なディレクトリまたはファイル名であることを確認しません。
任意のディレクトリ、ファイル名を指定するときは、
実行者自身が安全な名前であることを保証する必要があります。

### バグなどについて

issue を参照してください。

## ScreenShot

![](https://github.com/XJINE/Unity3D_ImageCaptureTool/blob/master/screenshot.png)
