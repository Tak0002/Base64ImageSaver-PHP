Base64ImageSaver-PHP
====================

Save base64 images in HTML and replace base64 to the image path.

HTML中に含まれるBase64形式の画像を、外部ファイル（一般的な画像ファイル）に出力し、HTML中のbase64形式で記述されている画像を出力した画像へのURLに書き換えます。



使い方
=========================

コンストラクタで画像を保存するディレクトリを指定します。
saveImagesメソッドにbase64形式の画像が含まれるHTMLファイルを引数に入れると、指定したディレクトリに保存された画像を呼び出すように置換されたHTMLが返ってきます。

```php
$imageSaver = new ImageSaver('img/'); //画像を保存するディレクトリを指定
$html = $imageSaver->saveImages($originalHTML); 
```


ライセンス
======================

The MIT License (MIT)