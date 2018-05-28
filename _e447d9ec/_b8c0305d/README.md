* [Haskell でソケット通信をやってみる](http://yasutech.blogspot.jp/2012/01/haskell.html)
* [msgpack/msgpack-haskell](https://github.com/msgpack/msgpack-haskell)
* [Hakyll](http://jaspervdj.be/hakyll/)
* [websockets](http://jaspervdj.be/websockets/)
* [egonSchiele/HandsomeSoup](https://github.com/egonSchiele/HandsomeSoup)
* [jwiegley/github](https://github.com/jwiegley/github)
* [Deploying Haskell to Heroku using Docker](http://www.reddit.com/r/haskell/comments/35he88/deploying_haskell_to_heroku_using_docker/)
* [Haskell on Heroku](https://haskellonheroku.com/)
* [fb](https://hackage.haskell.org/package/fb)

##Database
* [Safe concurrent MySQL access in Haskell](https://ro-che.info/articles/2015-04-17-safe-concurrent-mysql-haskell)
* [Haxl - Haskellを使った暗黙的な並列データアクセス](http://www.infoq.com/jp/news/2014/06/haxl)
* [esqueleto](http://hackage.haskell.org/package/esqueleto)
* [postgresql-simple](https://hackage.haskell.org/package/postgresql-simple)

##JSON
* [aeson](http://hackage.haskell.org/package/aeson)
  * [Aeson: the tutorial](http://artyom.me/aeson)
* [aeson-schema](https://hackage.haskell.org/package/aeson-schema)
  * [timjb/aeson-schema](https://github.com/timjb/aeson-schema)
* [buffer-builder](https://hackage.haskell.org/package/buffer-builder)

##Client
* [HTTP](https://hackage.haskell.org/package/HTTP) - HTTPSは対応していない
* [wreq](http://www.serpentine.com/wreq/)
* [http-conduit](http://hackage.haskell.org/package/http-conduit)
* [twitter-conduit](http://hackage.haskell.org/package/twitter-conduit)

##HTML Template/DSL
* Template - [shakespeare](https://hackage.haskell.org/package/shakespeare)
* [blaze-html](http://hackage.haskell.org/package/blaze-html)

###Lucid
* [chrisdone/lucid](https://github.com/chrisdone/lucid)
* [Lucid: templating DSL for HTML](http://chrisdone.com/posts/lucid)

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

##Server
* [mighttpd](https://hackage.haskell.org/package/mighttpd)
* [Haskell から見た node.js](http://d.hatena.ne.jp/kazu-yamamoto/20110825/1314254885)
* [Web](http://www.scs.stanford.edu/14sp-cs240h/slides/web-slides.lhtml)
* [agrafix/Spock](https://github.com/agrafix/Spock)
* [Overloading Monads for Html Deployment](https://www.fpcomplete.com/user/AthanClark/overloaded-monadic-deployment)

###WAI/Warp
* [wai](https://hackage.haskell.org/package/wai)
* [warp](https://hackage.haskell.org/package/warp)

###Scotty
* [scotty-web/scotty](https://github.com/scotty-web/scotty)

###Servant
* [servant](http://haskell-servant.github.io/)

###Yesod
* [Yesod Web Framework](http://www.yesodweb.com/)
* [quick start guide](http://www.yesodweb.com/page/quickstart)
* [tutorial](http://yannesposito.com/Scratch/en/blog/Yesod-tutorial-for-newbies/)
* [i18n, authentication, authorization, and database](http://www.yesodweb.com/blog/2012/01/blog-example)
* [book](http://www.yesodweb.com/book)
* [cookbook](https://github.com/yesodweb/yesod/wiki/Cookbook)
* [Getting started with Yesod using Docker](https://ilikewhenit.works/blog/1)
