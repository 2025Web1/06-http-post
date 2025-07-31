---
sort: 7
---

# 課題の解答

以下は、課題の解答例です。
課題に合格されなかった方は、こちらのコードを参考にしてください。

**password.html**

```php
<!DOCTYPE html>
<html lang="ja">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>パスワードの練習課題</title>
</head>

<body>
    <h4>パスワード練習課題</h4>
    <form method="POST" action="password.php">
        ユーザーID：<input type="text" name="user"><br>
        パスワード：<input type="password" name="pass"><br>
        <input type="submit" name="submit" value="送信">
    </form>
</body>

</html>
```

**password.php**

```php
<!DOCTYPE html>
<html lang="ja">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>パスワードの練習(送信後)</title>
</head>

<body>

    <h4>パスワード練習課題</h4>
    <?php
    echo '<p>入力されたユーザーIDは、' . $_POST['user'] . 'です。</p>';
    echo '<p>入力されたパスワードは、' . $_POST['pass'] . 'です。</p>';
    ?>
    <a href='password.html'>戻る</a>
</body>

</html>
```

**pulldown.html**

```php
<!DOCTYPE html>
<html lang="ja">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>プルダウンの練習</title>
</head>

<body>
    <h4>プルダウン練習課題</h4>
    あなたの好きなフルーツを選んでください。<br>
    <form method="POST" action="pulldown.php">
        <select name="fruit">
            <option>オレンジ</option>
            <option>リンゴ</option>
            <option>メロン</option>
        </select>
        <input type="submit" name="submit" value="送信">
    </form>
</body>

</html>
```

**pulldown.php**

```php
<!DOCTYPE html>
<html lang="ja">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>プルダウンメニューの練習(結果)</title>
</head>

<body>
    <h4>プルダウン練習課題</h4>
    <?php
    echo '<p>あなたの好きなフルーツは、' . $_POST['fruit'] . 'ですね。</p>';
    ?>
    <a href='pulldown.html'>戻る</a>
</body>

</html>
```

**textarea.html**

```php
<!DOCTYPE html>
<html lang="ja">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>テキストエリアの練習問題</title>
</head>

<body>
    <h4>テキストエリア練習課題</h4>
    <form method="POST" action="textarea.php">
        <textarea name="input_text" rows="4" cols="50"></textarea><br>
        <input type="submit" name="submit" value="送信">
    </form>

</body>

</html>
```

**textarea.php**

```php
<!DOCTYPE html>
<html lang="ja">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>テキストエリア練習問題(結果)</title>
</head>

<body>
    <h4>テキストエリア練習課題</h4>
    <p>入力された文章は、つぎのとおりです。</p>
    <?php
    // 【補習用穴埋め】$_POST['　　　　　']の'　　　　　'部分を埋めてください。
    // ヒント：textareaのname属性を確認してください。
    echo '<p>' . $_POST['          '] . '</p>';
    ?>
    <a href='textarea.html'>戻る</a>

</body>

</html>
```
