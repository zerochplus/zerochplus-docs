---
title: admin.cgiにログインすることはできたが、項目をクリックするとログイン画面に戻される
date: 2017-02-12 20:42:30 +0900
cgiver: 0.7.4
---

サーバの仕様・設定に対して、パーミッションの設定が適切でない可能性があります。 [Permission](https://ja.osdn.net/projects/zerochplus/wiki/Permission)をよくお読みになり、適切に設定を行ってください。

「サーバが非suEXECなのに、パーミッションはsuEXEC有効時のものを設定している」などといった可能性があります。 suEXECのsの字もわからない人は[KENT大先生の解説](http://www.kent-web.com/support/faq.html#q15)を見てください。

「test/info/.session/」ディレクトリは、UNIX・Linuxでは隠しファイル扱い(ドットファイル)のため、FTPクライアントで表示されていない可能性があります。 もし見当たらない場合は、ドットファイルが表示される設定になっているかを確認してみてください。
