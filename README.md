# Name
フォルダ内Excelシート書出ツール（FSO再帰処理）.xlsm
## Overview
1.「フォルダ名・Excelファイル名・内包シート名」の書き出し  
2.Excelシート名リストによる1シートへの全シートデータ書き出し  
の機能を持ったツールです。
## Usage
### 機能別使用方法
#### 1.起点フォルダ以下のフォルダ名-Excelファイル名-シート名書き出し機能
「シート名検査」シートに実装。2つめの機能を運用するための補助機能。（再帰処理を使用）  
「起点フォルダ」にフルパスを入力し、「シート名書出」を押下することで、そのフォルダ以下にある全フォルダ内のExcelファイルを探査し、シート名を書き出す。（シート数制限：10）  
※ディレクトリ構造によっては処理に多大な時間を要する可能性あり。  
#### 2.フォルダ名-Excelファイル名-シート名指定によるシート内容の書き出し機能
1の機能によって得たフォルダ-ファイル-シート（シートが複数ある場合は1つを選択）の名前データをリスト入力し、「シート展開書出」を押下することで、「展開書出」シートにリストにある全シート内容を転記する。  
※A列を主キー、1行目を見出しとしたテーブルデータの書き出しを想定しているため、それ以外の形式のシートが書き出し対象に含まれる場合、正常に書き出しが実行されない可能性があります（最下最右計算関係）  
