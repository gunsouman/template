# Features

アプリケーションの概要

[![NPM version][shield-npm]](#)
[![Node.js version support][shield-node]](#)
[![Build status][shield-build]](#)
[![Code coverage][shield-coverage]](#)
[![Dependencies][shield-dependencies]](#)
[![MIT licensed][shield-license]](#)



[shield-coverage]: https://img.shields.io/badge/coverage-100%25-brightgreen.svg
[shield-dependencies]: https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg
[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
[shield-node]: https://img.shields.io/badge/node.js%20support-0.10–5-brightgreen.svg
[shield-npm]: https://img.shields.io/badge/npm-v3.2.0-blue.svg
[shield-build]: https://img.shields.io/badge/build-passing-brightgreen.svg

# Requirements
利用する外部ライブラリ（nodeのpackageのようにバージョン管理の仕組みがある場合は使用しない）
* pandas    1.0.1
* ipython   7.12.0
* numpy     1.18.1
* openpyxl  3.0.3


# Installation
外部ライブラリのインストール（nodeのpackageのようにバージョン管理の仕組みがある場合は使用しない）
```bash
pip install pandas
pip install ipython
pip install numpy
pip install openpyxl
```
 
 
# Usage
 使い方説明
 1.初回実行時「default.config.json」内の"通知先(e-mail)"を変更し、通知先を設定する。
 2.pyプログラムを実行する。
 
```bash
python send_alert_report.py

```
分析サーバーの場合、pythonコマンドのバージョンが異なるため、上記に変わり下記を実行してください
```bash
/opt/anaconda3/envs/P37C0/bin/python send_alert_report.py
```


# Note
 備考
 ・本ソースは、IoTイノベ室の分析サーバー専用に実装されている箇所があります。
   - 分析サーバーにマウントされている、NAS上のWorkMateのログを用いております。
   - 実装している分析サーバーでは、本プログラムを実行前に、WorkMateのログを事前に更新するように処理を行っております。
   - (python /mnt/landisk0/data/WorkMate/scripts/00_import_logs/app.py)
 
 ・本ソースはipynbをベースに開発をしています。修正を行う場合はipynbを編集し下記のコマンドを実行してipynbをpy形式で出力してください。
```bash
sh build.sh
```
 ・「send_deficit_data_report.ipynb」は欠損が多いデバイスを通知する機能ですが、現在未実装です
 
# Author
 
* 作成者:大貫 誠
* 所属：IoTイノベーション室
* E-mail：m-onuki@uniteq.co.jp
 
 
# License
-------

Paddington is licensed under the [MIT](#) license.  
Copyright &copy; 2023, Rowan Manning


参考文献：https://gist.github.com/rowanmanning/77f31b2392dda1b58674
