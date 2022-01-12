# JavaScript-DOM
## JavaScript学習
1. DOM操作
- Webサイトを動的に置き換える技術
- Document Object Model(DOM)という、HTMLやXMLをアプリケーションから操作するための仕組みを利用
2. DOMツリー<br>
HTMLドキュメントやXMLドキュメントをツリー構造として表現したもの
3. ノード<br>
文章を構成する要素、属性、テキストといったオブジェクトをノードという
4. IDをキーに要素を取得<br>
- getElementByldメゾット
- (概要)指定したidを持つ要素を1つ取得する
- (構文)document.ElementByld(id)
5. タグ名をキーに要素を取得<br>
- getElementsByNameメゾット
- (概要)指定したタグ名を持つ要素を取得するメゾット
- (構文)document.getElementsByTagName
6. name属性をキーに要素を取得
- getElementsByNameメゾット
- (概要)指定したname属性を持つ要素を取得するメゾット
- ラジオボタン、チェックボタンなどのname属性が等しい要素群の取得に利用
- (構文)document.getElementsByName(name)
7. class属性をキーに要素を取得
- (概要)指定したclass属性を持つ要素を取得するメゾット
- (構文)document.getElementsByClassName(name)
8. ノード追加
- 要素/テキストノードの作成
- ノード同士を組み立て、ドキュメントに追加
9. createElemntメゾット
- (概要)要素を作成する
- (構文)document.createElement(name)
9. appendChildメゾット
- (説明)指定された要素を現在の最後の子養子として追加
- (構文)element.appendChild(node)
10. replaceChildメゾット
- (概要)指定した子ノードを置き換える
- (構文)replaceNode = parentNode.replaceChild(newChild, oldChild)
11. removeChildメゾット
- (概要)指定した子ノードを取り除く
- (構文)oldChild = element.removeChild(child)
12. インベントとイベントハンドラを関連付け（タグ）
- 開始タグの中で関連つける方法
- (構文)<要素名 on イベント名="イベントハンドラ">...</要素名>
13. インベントとイベントハンドラを関連付け（プロパティ）
- プロパティを使って関連付ける方法
- (構文) オブジェクト名.onイベント名 = function() {
  // イベントハンドラ
};
14. loadイベント
- 関連づけられた要素を読み終わった時に発生するイベント
- 画像を含む、ページが完全に読み終わったことを検知して、何らかの処理を実行したいときに使用
15. addEventListenerメゾット
- 1つの要素や1つのイベントに対して、複数のイベントハンドラを設定できる。
- onxxxxx(onclick等)では、1つの要素や1つのイベントに対して、1つのイベントハンドラしか設定できない問題。
- シンプルなアプリなら良いが、複雑なアプリを開発するときに、問題になってくる。
- onxxxxx(onclick等)では、本来レイアウトを定義するべきHTMLの中に、javascriptのコードを混在させており、可能性が落ちる(モダンではない書き方)
- (構文)要素オブジェクト.addEventListener(イベントの種類, function() {
  イベントハンドラ
}, false);