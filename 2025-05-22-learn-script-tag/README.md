
# 📚 JavaScriptの基本：scriptタグ

<br>

## 🗓️ 日付
2025-05-22

<br>

## 🎯 今回の目的
JavaScriptをHTMLに記述して動かす基本的な方法を理解する。

<br>

## 💻 利用シーン
- ブラウザ上でJavaScriptを動かすとき
- HTMLに直接スクリプトを埋め込みたいとき

<br>

## 🔣 基本構文
```html
<script>
  // JavaScriptコードを書く
</script>
```

<br>

## ✏️ 基本的な使い方
-  <script>タグは基本的に<body>の終わりに置くのが望ましい（HTMLの読み込み後に動作させるため）。
- JavaScriptの関数を作り、HTMLのイベント（ボタンのクリックなど）に紐づける。

<br>

## 📂 使用ファイル
- `index.html`：HTMLの基本構造とscriptの使い方・実用例

  <br>
  
## 💡 実用例の一部
```html
<body>

  <!-- ボタンをクリックすると changeText 関数が実行される -->
  <button onclick="changeText()">クリック</button>

  <!-- テキストを変更する対象の要素 -->
  <p id="text">元の文字</p>

  <script>
    // changeText 関数は、ボタンがクリックされたときに呼び出される
    function changeText() {
      // デバッグ用：アラートを表示して関数が呼ばれたことを確認
      alert("ボタンが押されました！");

      // id="text" の要素のテキストを変更する
      document.getElementById("text").textContent = "変更後の文字";
    }
  </script>

</body>
```

### 📝 解説ポイント

- `onclick` 属性でイベント実行
- `alert()` は処理を一時停止して状態を確認できる
- `document.getElementById("text")` で、HTMLの特定の要素にアクセス
- `textContent` でテキストを書き換える

<br>

## 🔗 類似メソッド・関連情報
- `console.log()`：開発者ツールで値を表示
- addEventListener()：イベント登録の標準的な書き方

<br>

## 📝 振り返り・ポイントまとめ
- 初心者はまず <script> タグを理解し、簡単な動作を試すことが大切。
- alert() は処理を止めるデバッグに便利。
