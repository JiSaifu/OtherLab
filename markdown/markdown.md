# Markdown記法のいろいろお試し
参考元：[Markdown記法 サンプル集](https://qiita.com/tbpgr/items/989c6badefff69377da7)

## <font color="red">見出し</font>
- 記法：
```Markdown
<!-- # + ' '(スペース) + Header内容 -->
# これはH1タグです
## これはH2タグです
### これはH3タグです
```
- 結果：
<!-- # + ' '(スペース) + Header内容 -->
# これはH1タグです
## これはH2タグです
### これはH3タグです
***

## <font color="red">番号付きリスト</font>
- 記法：
```Markdown
<!--
    1.(次の番号の場合でも「1.」になる) + ' '(スペース) + リスト内容
    ネストリストの場合、1.の前にタブを入れる
-->
1. リスト1
    1. ネストリスト1_1
    1. ネストリスト1_2
1. リスト2
```
- 結果：
<!--
    1.(次の番号の場合でも「1.」になる) + ' '(スペース) + リスト内容
    ネストリストの場合、1.の前にタブを入れる
-->
1. リスト1
    1. ネストリスト1_1
    1. ネストリスト1_2
1. リスト2
***

## <font color="red">箇条書きリスト</font>
- 記法：
```Markdown
<!--
    - + ' '(スペース) + リスト内容
    ネストリストの場合、「-」の前にタブを入れる
-->
- リスト1
    - ネストリスト1_1
        - ネストリスト1_1_1
        - ネストリスト1_1_2
            - ネストリスト1_1_1_1
        - ネストリスト1_1_3
    - ネストリスト1_2
- リスト2
```
- 結果：
<!--
    - + ' '(スペース) + リスト内容
    ネストリストの場合、「-」の前にタブを入れる
-->
- リスト1
    - ネストリスト1_1
        - ネストリスト1_1_1
        - ネストリスト1_1_2
            - ネストリスト1_1_1_1
        - ネストリスト1_1_3
    - ネストリスト1_2
- リスト2
***

## <font color="red">引用</font>
- 記法：
```Markdown
<!-- > + ' '(スペース) + 引用の内容 -->
> お世話になっております。XXXです。
> ご連絡頂いたバグの件ですが、仕様です。
```
- 結果：
<!-- > + ' '(スペース) + 引用の内容 -->
> お世話になっております。XXXです。  
> ご連絡頂いたバグの件ですが、仕様です。
***

## <font color="red">二重引用</font>
- 記法：
```Markdown
<!-- >> + ' '(スペース) + 二重引用の内容 -->
> お世話になっております。XXXです。
> ご連絡頂いたバグの件ですが、仕様です。
>> お世話になっております。YYYです。
>> あの新機能バグっているですね。
```
- 結果：
<!-- >> + ' '(スペース) + 二重引用の内容 -->
> お世話になっております。XXXです。
> ご連絡頂いたバグの件ですが、仕様です。
>> お世話になっております。YYYです。
>> あの新機能バグっているですね。
***

## <font color="red">pre記法(スペース4 or タブ)</font>
- 記法 & 結果：
<!-- 半角スペース4 or タブを行の先頭に入れて、コードブロックのpre表示できる -->
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
先頭の半角スペース or タブを消すことで、通常モードに戻る

    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
***

## <font color="red">code記法</font>
- 記法：
```Markdown
<!-- バッククォートで文字列を囲む -->
インストールコマンド`gem install hoge`です。
```
- 結果：  
インストールコマンド`gem install hoge`です。
***

## <font color="red">強調:\<em></font>
- 記法：
```Markdown
<!-- * or _(アスタリスク or アンダースコア)で文字列を囲む -->
normal *italic* normal  
normal _italic_ normal
```
- 結果：  
normal *italic* normal  
normal _italic_ normal
***

## <font color="red">強調:\<strong></font>
- 記法：
```Markdown
<!-- * or _(アスタリスク or アンダースコア)2個で文字列を囲む -->
normal **bold** normal  
normal __bold__ normal
```
- 結果：  
normal **bold** normal  
normal __bold__ normal
***

## <font color="red">強調:\<em>+\<strong></font>
- 記法：
```Markdown
<!-- * or _(アスタリスク or アンダースコア)3個で文字列を囲む -->
normal ***italic + bold*** normal  
normal ___italic + bold___ normal
```
- 結果：  
normal ***italic + bold*** normal  
normal ___italic + bold___ normal
***

## <font color="red">水平線</font>
- 記法：
```Markdown
<!-- * or _ or -(アスタリスク or アンダースコア or ハイフン)3個連続(スペースあってもOK)で文字列を囲む -->
** *
___
---
```
- 結果：  
** *
___
---
***

## <font color="red">リンク</font>
- 記法：
```Markdown
<!-- [表示文字](リンクURL)形式でリンクを記述できる -->
[Gooogle先生](https://www.google.co.jp/)
```
- 結果：  
[Gooogle先生](https://www.google.co.jp/)
***

## <font color="red">定義参照リンク</font>
- 記法：
```Markdown
<!--
    Markdownの文書の途中に長いリンクを記述したくない場合は、
    同じリンクの参照を何度も利用する場合は、リンク先への参照を定義することができる
-->
[Google先生][google]  
その他の文章  
[Google先生][google]  
[google]: http://www.google.co.jp/
```
- 結果：  
[Gooogle先生][google]  
その他の文章  
[Gooogle先生][google]  
[google]: http://www.google.co.jp/
***