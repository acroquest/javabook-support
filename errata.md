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
|3|p.78 「StaticTestMain.java」のコード（2カ所）|instanceFiled|instanceField|2017/05/01|
|3|p.78 「StaticTestMain.java」のコード 16L|System.out.println(test.instanceMethod()); // Hi Murata yay!|System.out.println(test.instanceMethod()); // Hi Okada yay!|2017/05/02|
|3|p.82 「3-2-7 インタフェース」中央|インタフェースは必ずpublicになるため、インタフェース名の前に書くpublicは省略することができます。ただ、筆者はpublicであることを明示するため、常にpublicをつけるようにしています。|（削除）|2017/04/18|
|3|p.90 「3-3-2 オブジェクトの等価性」中央 hashCodeメソッドのコード2行目|private int employeNo;|private int employeeNo;|2017/05/19|
|3|p.90 「3-3-2 オブジェクトの等価性」中央 hashCodeメソッドのコード11行目|result = prime * result + employeNo;|result = prime * result + employeeNo;|2017/05/19|
|4|p.108 「4-1-1 配列の基本を理解する」 中央のコード|int fib1 = 1;<br>int fib2 = 1;|int fib0 = 0;<br>int fib1 = 1;<br>int fib2 = fib0 + fib1;|2017/04/18|
|4|p.116 Note「Comparatorか、Comparableか？」のコード|public Student2(String name, int score) {|public Student(String name, int score) {|2017/05/19|
|4|p.116 Note「Comparatorか、Comparableか？」のコード|public int compareTo(Student2 o) {|public int compareTo(Student o) {|2017/05/19|
|4|p.126 「4-3-3 Listの代表的なメソッド」 の実行結果|⑧Shinが含まれているか：true|⑧Shinが含まれているか：false|2017/05/01|
|4|p.129 「4-3-6 Listのイテレーション」中央のコード|for (Iterator iterator = list.iterator(); iterator.hasNext(); ) {|for (Iterator&lt;String&gt; iterator = list.iterator(); iterator.hasNext(); ) {|2017/05/08|
|4|p.134 表「Mapインタフェースでの要素の取得、変換」の「メソッド名」「役割」「説明」|valueSet　値の集合の取得　Mapないのすべての要素の値の集合を取得する|values　値のコレクションの取得　Map内のすべての要素の値のコレクションを取得する|2017/04/18|
|4|p.145 Note「MapとSetの関係」|通常は boolean 型で「TRUE」が格納されます。この boolean 値は、使用されることはありません。|通常は Boolean 型で「TRUE」が格納されます。この Boolean 値は、使用されることはありません。|2017/04/22|
|5|p.150 「5-1-1 Stream APIでコレクションの操作はどう変わるか」のコード|//「中間操作」。score が 70 より大きい Student の抽出|//「中間操作」。score が 70 以上の Student の抽出|2017/05/01|
|5|p.153 「関数型インタフェースの代替として使用する」のコード|students.forEach(s -><br>&nbsp;&nbsp;&nbsp;&nbsp;System.out.println(s.getName() + ":" + s.getScore()));|Arrays.stream(students).forEach(s -><br>&nbsp;&nbsp;&nbsp;&nbsp;System.out.println(s.getName() + ":" + s.getScore()));|2017/04/23|
|5|p.162 「5-3-1 要素を置き換える中間操作」の説明文|このFunctionような代入先となる関数型インタフェースを引数に持つことで、|このFunctionのような代入先となる関数型インタフェースを引数に持つことで、|2017/05/22|
|6|p.197 (2)ラムダ式の中で発生した例外の扱い|ラムダの中に記述した処理で例外が発生する可能性があります。それが検査例外だった場合は、捕捉しないと、コンパイルエラーが発生します。|ラムダの中に記述した処理で例外が発生する可能性があります。特にStream APIで利用する、java.util.functionパッケージにある関数型インタフェースに対するラムダ式の場合、ラムダ式内で発生する例外が検査例外だった場合は、捕捉しないと、コンパイルエラーが発生します。|2017/04/18|
|6|p.199 表「Optional クラスが持つおもなメソッド」|optional.isPresent(value -> {...})|optional.ifPresent(value -> {...})|2017/05/01|
|6|p.183 (2)try-with-resources|じつはJava 7から、InputStreamなどのリソースを扱うクラスは、java.lang.AutoClosableインタフェースまたはjava.io.Closableインタフェースを実装するようになりました（java.io.Closableインタフェースは、java.lang.AutoClosableインタフェースを継承しています）。|じつはJava 7から、InputStreamなどのリソースを扱うクラスは、java.lang.AutoCloseableインタフェースまたはjava.io.Closeableインタフェースを実装するようになりました（java.io.Closeableインタフェースは、java.lang.AutoCloseableインタフェースを継承しています）。|2017/04/18|
|7|p.207 「7-1-4 複数の文字列を連結する」|「Listオブジェクトに保持した文字列を、カンマ（,）区切りで連結して表示する」|「Listオブジェクトに保持した文字列を、スペース区切りで連結して表示する」|2017/05/25|
|7|p.207 「7-1-4 複数の文字列を連結する」|「StringBuilderクラスを用いて、for文でListオブジェクトの要素とカンマを順に結合していく」|「StringBuilderクラスを用いて、for文でListオブジェクトの要素とスペースを順に結合していく」|2017/05/25|
|7|p.208 「7-1-4 複数の文字列を連結する」|しかし、この方法では、最後の要素の後にもカンマが結合されてしまうため、最後のカンマを除去する必要があるなど、|しかし、この方法では、最後の要素の後にもスペースが結合されてしまうため、最後のスペースを除去する必要があるなど、|2017/05/25|
|8|p.231 「Java 7以降でバイナリファイルを読み込むには」のコード|for (int ch; (ch = stream.read()) != -1; ) {|for (int ch; (ch = is.read()) != -1; ) {|2017/04/25|
|8|p.233 表「OpenOption の指定例 1」|DELETE_ON_CLOSE の行|（削除）|2017/05/01|
|8|p.236 「Java 6以前でテキストファイルに書き込むには」のコード|} catch (FileNotFoundException ex) {<br>&nbsp;&nbsp;&nbsp;&nbsp;//(3)ファイルそのものが存在しない場合<br>&nbsp;&nbsp;&nbsp;&nbsp;System.err.println(ex);<br><br>} catch (IOException ex) {<br>&nbsp;&nbsp;&nbsp;&nbsp;//(4)ファイルの読み込みに失敗した場合<br>&nbsp;&nbsp;&nbsp;&nbsp;System.err.println(ex);<br><br>} finally {<br>&nbsp;&nbsp;&nbsp;&nbsp;//(5)ファイルのクローズ処理|} catch (IOException ex) {<br>&nbsp;&nbsp;&nbsp;&nbsp;// (3)ファイルの書き込みに失敗した場合<br>&nbsp;&nbsp;&nbsp;&nbsp;System.err.println(ex);<br><br>} finally {<br>&nbsp;&nbsp;&nbsp;&nbsp;// (4)ファイルのクローズ処理|2017/05/01|
|8|p.239 「8-3-1 ファイルをコピーする」のコード|FileInputStream inputStream = new FileInputStream("C:/work/sample.dat");<br>FileOutputStream outputStream = new FileOutputStream("C:/work/copy.dat");<br><br>inputChannel = inputStream.getChannel();<br>outputChannel = outputStream.getChannel();|FileInputStream inputStream = new FileInputStream("C:/work/sample.dat");<br>inputChannel = inputStream.getChannel();<br><br>FileOutputStream outputStream = new FileOutputStream("C:/work/copy.dat");<br>outputChannel = outputStream.getChannel();|2017/05/01|
|8|p.253 図「staff.xml をツリー構造で表すと」|Document-Element(staff)|Document-Element(staffs)|2017/04/29|
|8|p.256 頭のソースコード 8L|parser = factory.newSAXParser();|（削除）|2017/05/01|
|9|p.286 「DateTimeParseException 例外が発生します」の実行結果|java.time.format.DateTimeParseException: Text '2017-02-25 19:09:59' could not be parsed at index 4|java.time.format.DateTimeParseException: Text '2017/02/25' could not be parsed at index 10|2017/04/29|
|12|p.352 「12-2-2 Builderパターン　〜複合化されたインスタンスの生成過程を隠ぺいする」のコード|（追加）|■TopPage.java<br>public class TopPage extends Page {<br>&nbsp;&nbsp;&nbsp;&nbsp;// 内容はPageと同じ。<br>}|2017/05/01|
|12|p.354 「12-2-3 Singletonパターン　～あるクラスについて、インスタンスが単一であることを保証する」のコード|return instance|return instance;|2017/04/25|
|13|p.378 「13-1-2 Mavenの基本的な利用方法」のディレクトリ構成<br><br>※ディレクトリ修正版のソースコードは https://github.com/acroquest/javabook-maven-example/tree/%2322|src/main/java/com/java/book/app/App.java<br>src/test/java/com/java/book/app/AppTest.java|src/main/java/jp/co/acroquest/javabook/maven/App.java<br>src/test/java/jp/co/acroquest/javabook/maven/AppTest.java|2017/05/03|
|13|p.379、p.382 pom.xmlサンプル|&lt;groupId&gt;com.java.book.app&lt;/groupId&gt;<br>&lt;url&gt;[http://maven.apache.org](http://maven.apache.org)&lt;/url&gt;|&lt;groupId&gt;jp.co.acroquest.javabook&lt;/groupId&gt;<br>&lt;url&gt;[https://github.com/acroquest/javabook-maven-example](https://github.com/acroquest/javabook-maven-example)&lt;/url&gt;|2017/05/03|
|13|p.399、p.400 「13-5-2 テストコードを実装する」のコード|package acroquest.java.junit;|package jp.co.acroquest.javabook.junit;|2017/05/03|
|14|p.430 「(2)ログ出力コードの記述」のコード|package acroquest.java.log;|package jp.co.acroquest.javabook.log;|2017/05/03|
|14|p.430、p.431 ログ出力例|2016-05-01 12:34:56,789 [main] INFO acroquest.java.log.LogbackSample - アプリケーションを実行しました。|2016-05-01 12:34:56,789 [main] INFO jp.co.acroquest.javabook.log.LogbackSample - アプリケーションを実行しました。|2017/05/03|
|14|p.432 logback.xml|&lt;logger name="acroquest.java.log.dao" level="DEBUG" /&gt;|&lt;logger name="jp.co.acroquest.javabook.log.dao" level="DEBUG" /&gt;|2017/05/03|
|索引|p.437|AutoClosableインタフェース<br>Closableインタフェース|AutoCloseableインタフェース<br>Closeableインタフェース|2017/04/18|
|索引|p.438|（DELETE_ON_CLOSEのページ数）233|246|2017/05/01|
|索引|p.441|valueSetメソッド|valuesメソッド|2017/04/18|
|著者略歴|p.446 谷本 心|関西 Java エンジニアの立ち上げや、|関西 Java エンジニアの会の立ち上げや、|2017/04/22|
