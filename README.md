# JavaScript-1
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
- ラジオぼたん、チェックボタンなどのname属性が等しい要素群の取得に利用
- (構文)document.getElementsByName(name)
7. class属性をキーに要素を取得
- (概要)指定したclass属性を持つ要素を取得するメゾット
- (構文)document.getElementsByClassName(name)