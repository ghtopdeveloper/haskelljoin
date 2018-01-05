* [シンプルでかつ最高のJavaScriptプロファイラ sjsp を作りました！](http://itchyny.hatenablog.com/entry/2015/07/01/120000)
* webfont generator - [ananthakumaran/webify](https://github.com/ananthakumaran/webify)
* [LambdaCms](http://lambdacms.org/)
* [Animating Web UI with React and Haskell](http://joelburget.com/react-haskell/)
* [A Distributed Haskell for the Modern Web](http://ekblad.cc/lic.pdf)

##Elm
* [elm](http://elm-lang.org/)
* [Evan Czaplicki - Let's be mainstream! User focused design in Elm - Curry On](https://www.youtube.com/watch?v=oYk8CKH7OhE)
* [elm-bridge](http://hackage.haskell.org/package/elm-bridge)
* [elm-lang/elm-make](https://github.com/elm-lang/elm-make)
* [elm+electronで気楽に始めるFRP](http://qiita.com/yasuyuky/items/e28106e3dd7fed17d50f)
* [関数型リアクティブプログラミング言語Elmに学ぶ フロントエンド開発の新しい形](http://codezine.jp/article/detail/8873)
* [Building elm with stack](http://therning.org/magnus/posts/2015-10-13-000-building-elm-with-stack.html)

##AltJS
* [Haskell風AltJSのベンチマーク](http://qiita.com/philopon/items/1451f6b8c5ccec41479d)
* [Haste](http://haste-lang.org/)
  * [Client-side haskell](http://ifeanyi.co/posts/client-side-haskell/)
* <http://lesguillemets.github.io/fouricle/>
* [オートマトンで遊ぶやつを作った](http://myuon-myon.hatenablog.com/entry/2015/12/18/193654)
* [Automatoy](http://myuon.github.io/automatoy/)
* [ghcjs/ghcjs](https://github.com/ghcjs/ghcjs)
* [faylang/fay](https://github.com/faylang/fay)
* [Haskell + Haste で Fourier 級数の可視化](http://qiita.com/lesguillemets/items/dbd928237be3e6a1221d)
* [Haste + Parsec でブラウザ上で動く電卓をつくる](http://qiita.com/lesguillemets/items/b58e684a773fb4b5e4aa)
* [Zero config, no server Haste.App](http://haste-lang.org/blog/haste-standalone/)

###Pure Script
* <http://www.purescript.org/>
* [andyarvanitis/pure11](https://github.com/andyarvanitis/pure11)
* [Stack Safety for Free](http://functorial.com/stack-safety-for-free/index.pdf)
* [slamdata/purescript-halogen](https://github.com/slamdata/purescript-halogen)
* [実例によるPureScript](http://hiruberuto.bitbucket.org/purescript/)
* [purescript/purescript-free](https://github.com/purescript/purescript-free)
* [Flare](http://david-peter.de/articles/flare/)
* [Pursuit](http://pursuit.purescript.org/)
* [PureScript for the Haskeller](http://www.arow.info/blog/posts/2015-12-17-purescript-intro.html)

##HTML Template/DSL
* [shakespeare](https://hackage.haskell.org/package/shakespeare)
* [ede](https://hackage.haskell.org/package/ede)
* [mustache](https://hackage.haskell.org/package/mustache)

###Blaze
* [blaze-html](http://hackage.haskell.org/package/blaze-html)
* [meiersi/blaze-react](https://github.com/meiersi/blaze-react)

###Lucid
* [chrisdone/lucid](https://github.com/chrisdone/lucid)
* [Lucid: templating DSL for HTML](http://chrisdone.com/posts/lucid)
* [lucid-svg](http://hackage.haskell.org/package/lucid-svg)

```haskell
indexHtml :: Html ()
indexHtml = do
    doctype_
    html_ $ do
        head_ $ do
            title_ [] "Hello Lucid!"
            link_  [rel_ "stylesheet", type_ "text/css", href_ "/css/main.css"]
        body_ $ do
            h1_ [] "Lucid"
            p_  [] "Lorem ipsum dolor sit amet, consectetur adipiscing elit,"
            script_ [src_ "/js/main.js"] ("" :: Text)
```
