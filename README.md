# processing_templates

イライラ棒　自身（点）が壁や障害物に当たらずにゴールを目指すゲームです。　 

## Usage

キーボード操作　矢印キーで移動します。二つ以上の同時押し（斜め移動）も可能です。

## Code review

プログラムのベースは、
[ここ](https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q10161818675) を参考にしました。

キーボード操作にしたかったため、
[ここ](https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q12140122737) を参考にしました。

障害物の棒を回転させたかったため、
[ここ](http://9ryulabo.com/processing-learner/4-6.html)
を参考にしました。

斜めのラインを入れたかったため、
[ここ](https://www.oreilly.co.jp/books/9784873117737/)
を参考にしました。
kとlに範囲を与えて連続したラインを作成し、序盤でつまずく箇所を付け足しました。
```java
for (int k = 70;k < 450; k +=40){//ギザギザ線
    line(k,90,k+20,110);
    line(k-20,110,k,90);
}
for (int l = 70; l < 450; l +=40){
    line(l,70,l+20,90);
    line(l-20,90,l,70);
}

```

## License

The processing application is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
