# PukiWiki用プラグイン<br>CCライセンス表示 cc.inc.php

クリエイティブ・コモンズ・ライセンス4.0コモンズ証へのリンクアイコンを表示する[PukiWiki](https://pukiwiki.osdn.jp/)用プラグイン。

|対象PukiWikiバージョン|対象PHPバージョン|
|:---:|:---:|
|PukiWiki 1.5.3 ~ 1.5.4RC (UTF-8)|PHP 7.4 ~ 8.1|

## インストール

cc.inc.php を PukiWiki の plugin ディレクトリに配置してください。

## 使い方

```
#cc(by|by-sa|by-nd|by-nc|by-nc-sa|by-nc-nd[,scale])
&cc(by|by-sa|by-nd|by-nc|by-nc-sa|by-nc-nd[,scale]);
```

* 第1引数 … ライセンス種別。by, by-sa, by-nd, by-nc, by-nc-sa, by-nc-nd のいずれか
* scale … 表示スケール（百分率）。省略時の既定値は 100

## 使用例

```
#cc(by-nc-nd)
&cc(by-nc,150);
```

## 設定

ソース内の下記の定数で動作を制御することができます。

|定数名|値|既定値|意味|
|:---|:---:|:---|:---|
|PLUGIN_CC_COLOR|カラーコード文字列||アイコン色（例：'#FFFFFF'）。空なら黒|
