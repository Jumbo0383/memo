# 自分用メモ

## バージョン管理
tensorflow2.3 <br>
CUDA==10.1 <br>
CuDNN==7.6.5 <br>

## CUDA再インストール
Windowsの場合では，コントロールパネルから"cuda"と検索すると何種類かアプリケーションが出てくるので手動ですべて削除．<br>
tensorflow2.3の場合はCUDA10.1をインストール(以下URL)<br>
https://developer.nvidia.com/cuda-10.1-download-archive-base?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exenetwork

## CuDNNのインストール
以下サイトからCuDNNをインストールする． <br>
https://developer.nvidia.com/cudnn <br>
アカウント登録が必要ですがgoogleアカウントでもログイン可能です． <br>
いくつか質問に答えた後で，CUDAとOSに対応するCuDNNのインストールを行う． <br>
zipファイルのダウンロード後にファイルを解凍．<br>
CUDA/v10.1内に回答したファイルをコピペする．

## ReadTimeoutError が起きた場合
> pip --default-timeout=100 install tensorflow-gpu==2.3.0 <br>

でなんとかなる．

## Error code -9986 Internal PortAudio error
pythonプログラムとGatageBandなどオーディオデバイスを用いる複数のアプリを立ち上げているとなるので，一旦両方のアプリを落としてPythonプログラムをもう一度開けなすと動くはずです
