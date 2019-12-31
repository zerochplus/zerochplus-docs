---
title: Internal Server Errorが出る
date: 2019-08-11 23:20:50 +0900
cgiver: 0.7.4
---

エラーログ読んでください！お願いだから！  
エラーログも無しに質問されても答えようがないから！

もしエラーログが見られないレンタルサーバの場合、各.cgiファイルの十何行目にある↓の、行頭の「#」を(2個あれば2個とも)消せば、ブラウザ上にエラーの詳細が表示されるかと思います。たぶん^^;

> use CGI::Carp qw(fatalsToBrowser);

エラーが解消したら、「#」を元に戻しておきましょう。

何らかの理由でエラーログが表示できない、あるいはエラーログに書いてあることの意味が解らない場合、[Install](https://ja.osdn.net/projects/zerochplus/wiki/Install)ページにある「[表示されない場合](https://ja.osdn.net/projects/zerochplus/wiki/Install#h3-.E8.A1.A8.E7.A4.BA.E3.81.95.E3.82.8C.E3.81.AA.E3.81.84.E5.A0.B4.E5.90.88)」を確認すると良いでしょう。Internal Server Errorの3大原因が書いてあります。
