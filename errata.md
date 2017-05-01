# 『Java本格入門』の正誤表

下記の誤りがありました。お詫びして訂正いたします。

## 第1刷

|ch|頁|誤|正|update|
|---|---|---|---|---|
|2|p.35 表「ビット演算子」の「>>」行の「意味」列|右辺の数だけビットを右シフトする（算術シフト）。正負の符号を表すビットは保持し、それ以外の空いたビットは0埋めする|右辺の数だけビットを右シフトする（算術シフト）。空いたビットは、正負の符号を表すビットで埋めする|2017/04/13|
|2|p.36 中央|32ビットの数値を16ビット分右にシフトし、空いたビットは0で埋められるので、|32ビットの数値を16ビット分右にシフトし、空いたビットは正の符号を表す0で埋められるので、|2017/04/13|
|2|p.37 表「代入演算子」の「>>=」行「意味」列|右辺の数だけビットを右シフトする（算術シフト）。正負の符号を表すビットは保持し、それ以外の空いたビットは0埋めする|右辺の数だけビットを右シフトする（算術シフト）。空いたビットは、正負の符号を表すビットで埋めする|2017/04/13|
|3|p.63 表「プリミティブ型」の「boolean」行「サイズ」列|1bit|-|2017/04/22|
|3|p.70 3L|valueOfメソッドを利用した場合は、-127から128の範囲であれば|valueOfメソッドを利用した場合は、-128から127の範囲であれば|2017/04/22|
|3|p.77 「StaticTest.java」のコード（2カ所）|instanceFiled|instanceField|2017/05/01|
|3|p.82 「3-2-7 インタフェース」中央|インタフェースは必ずpublicになるため、インタフェース名の前に書くpublicは省略することができます。ただ、筆者はpublicであることを明示するため、常にpublicをつけるようにしています。|（削除）|2017/04/18|
|4|p.108 「4-1-1 配列の基本を理解する」 中央のコード|int fib1 = 1;<br>int fib2 = 1;|int fib0 = 0;<br>int fib1 = 1;<br>int fib2 = fib0 + fib1;|2017/04/18|
|4|p.126 「4-3-3 Listの代表的なメソッド」 の実行結果|⑧Shinが含まれているか：true|⑧Shinが含まれているか：false|2017/05/01|
|4|p.134 表「Mapインタフェースでの要素の取得、変換」の「メソッド名」「役割」「説明」|valueSet　値の集合の取得　Mapないのすべての要素の値の集合を取得する|values　値のコレクションの取得　Map内のすべての要素の値のコレクションを取得する|2017/04/18|
|4|p.145 Note「MapとSetの関係」|通常は boolean 型で「TRUE」が格納されます。この boolean 値は、使用されることはありません。|通常は Boolean 型で「TRUE」が格納されます。この Boolean 値は、使用されることはありません。|2017/04/22|
|5|p.153 「関数型インタフェースの代替として使用する」のコード|students.forEach(s -><br>&nbsp;&nbsp;&nbsp;&nbsp;System.out.println(s.getName() + ":" + s.getScore()));|Arrays.stream(students).forEach(s -><br>&nbsp;&nbsp;&nbsp;&nbsp;System.out.println(s.getName() + ":" + s.getScore()));|2017/04/23|
|6|p.197 (2)ラムダ式の中で発生した例外の扱い|ラムダの中に記述した処理で例外が発生する可能性があります。それが検査例外だった場合は、捕捉しないと、コンパイルエラーが発生します。|ラムダの中に記述した処理で例外が発生する可能性があります。特にStream APIで利用する、java.util.functionパッケージにある関数型インタフェースに対するラムダ式の場合、ラムダ式内で発生する例外が検査例外だった場合は、捕捉しないと、コンパイルエラーが発生します。|2017/04/18|
|6|p.183 (2)try-with-resources|じつはJava 7から、InputStreamなどのリソースを扱うクラスは、java.lang.AutoClosableインタフェースまたはjava.io.Closableインタフェースを実装するようになりました（java.io.Closableインタフェースは、java.lang.AutoClosableインタフェースを継承しています）。|じつはJava 7から、InputStreamなどのリソースを扱うクラスは、java.lang.AutoCloseableインタフェースまたはjava.io.Closeableインタフェースを実装するようになりました（java.io.Closeableインタフェースは、java.lang.AutoCloseableインタフェースを継承しています）。|2017/04/18|
|8|p.231 「Java 7以降でバイナリファイルを読み込むには」のコード|for (int ch; (ch = stream.read()) != -1; ) {|for (int ch; (ch = is.read()) != -1; ) {|2017/04/25|
|8|p.253 図「staff.xml をツリー構造で表すと」|Document-Element(staff)|Document-Element(staffs)|2017/04/29|
|8|p.256 頭のソースコード 8L|parser = factory.newSAXParser();|（削除）|2017/05/01|
|9|p.286 「DateTimeParseException 例外が発生します」の実行結果|java.time.format.DateTimeParseException: Text '2017-02-25 19:09:59' could not be parsed at index 4|java.time.format.DateTimeParseException: Text '2017/02/25' could not be parsed at index 10|2017/04/29|
|12|p.354 「12-2-3 Singletonパターン　～あるクラスについて、インスタンスが単一であることを保証する」のコード|return instance|return instance;|2017/04/25|
|索引|p.437|AutoClosableインタフェース<br>Closableインタフェース|AutoCloseableインタフェース<br>Closeableインタフェース|2017/04/18|
|索引|p.441|valueSetメソッド|valuesメソッド|2017/04/18|
|著者略歴|p.446 谷本 心|関西 Java エンジニアの立ち上げや、|関西 Java エンジニアの会の立ち上げや、|2017/04/22|
