#モナド交換子
* [Proper Treatment 正當作法/blog/posts/Monad transformers](http://conway.rutgers.edu/~ccshan/wiki/blog/posts/Monad_transformers/)
* [Composing Monads Using Coproducts](http://www.informatik.uni-bremen.de/~cxl/papers/icfp02.pdf)
* [monad-levels](http://hackage.haskell.org/package/monad-levels)
  * [Monadic yak shaving](https://ivanmiljenovic.wordpress.com/2015/02/02/monadic-yak-shaving/)
* [Monatron](https://hackage.haskell.org/package/Monatron)
* [Announcing: monad-unlift](https://www.fpcomplete.com/blog/2015/04/announcing-monad-unlift)
* [Ether - Monad Transformers and Classes](https://int-index.github.io/ether/)
* [Monad transformers and comonad transformers](http://dlaing.org/cofun/posts/monad_transformers_and_comonad_transformers.html)
* [Fusion for Free: Efficient Algebraic Effect Handlers](http://people.cs.kuleuven.be/~tom.schrijvers/portfolio/mpc2015.html)
* [Documentation.Layers.Overview](http://hackage.haskell.org/package/layers/docs/Documentation-Layers-Overview.html)

##Monad Transformer
* [transformers](https://hackage.haskell.org/package/transformers)
* [モナドトランスフォーマーとその周辺](http://qiita.com/ruicc/items/7512c990a1835bba444a)
* [Haskell モナド変換子 超入門](http://qiita.com/7shi/items/4408b76624067c17e933)
* [モナドトランスフォーマー・ステップ・バイ・ステップ](http://bicycle1885.hatenablog.com/entry/2012/12/08/165236)
* [A Gentle Introduction to Monad Transformers](https://github.com/kqr/gists/blob/master/articles/gentle-introduction-monad-transformers.md)
* [モナモナ言うモナド変換子入門](http://hiratara.github.io/presentations/2015-03-21_monadbase_vol2.html#/)
* [Monad transformer](http://mbps.hatenablog.com/entry/2014/06/28/033234)
* [Adjunction からの monad transformer](http://mbps.hatenablog.com/entry/2014/11/25/220948)
* [Monad からの monad transformer](http://mbps.hatenablog.com/entry/2014/12/11/112455)
* [Wrangling Monad Transformer Stacks](https://www.youtube.com/watch?v=8t8fjkISjus)
* [Monad transformers](http://taylor.fausak.me/2015/05/14/monad-transformers/)
* [The mmorph package](https://hackage.haskell.org/package/mmorph)
* [ContEitherT](https://iteratee.wordpress.com/2015/10/01/conteithert/)

transformersにはMonad Transformerを新しく定義する度に全ての組み合わせの実装を定義する必要があるという問題点がある。

###monad-control
* [モナドトランスフォーマーとmonad-control](http://maoe.hatenadiary.jp/entry/20111207/1323185162)
* [monad-control](https://hackage.haskell.org/package/monad-control)
* [lifted-base](https://hackage.haskell.org/package/lifted-base)

###ResourceT
* [resource-simple](https://hackage.haskell.org/package/resource-simple)

###Parser
* [parsec](https://hackage.haskell.org/package/parsec)
* [attoparsec](http://hackage.haskell.org/package/attoparsec)
* [trifecta](https://hackage.haskell.org/package/trifecta)

```haskell
type Parser = StateT String []
-- type Parser = StateT String Maybe
-- type Parser = StateT String (Either Error)

parse = evalStateT
```

* [モナディック・パーサー](http://d.hatena.ne.jp/kazu-yamamoto/20080920/1221881130)
* [構文解析器結合子](https://www.ipsj.or.jp/07editj/promenade/4702.pdf)
* [Monadic Parsing in Haskell](http://www.cs.nott.ac.uk/~gmh/pearl.pdf)
* [JavaScriptでパーサコンビネータのコンセプトを理解する](http://blog.anatoo.jp/entry/2015/04/26/220026)
* [cassava](https://hackage.haskell.org/package/cassava-0.4.2.4)
* [haskell-src-exts](https://hackage.haskell.org/package/haskell-src-exts)
* [Pandoc - a universal document converter](http://pandoc.org/)
  * [markup.rocks](http://markup.rocks/)
* [language-javascript](https://hackage.haskell.org/package/language-javascript)
* [language-python](https://hackage.haskell.org/package/language-python)
* [Alex and Happy: Parsing comments and strings](http://www.jyotirmoy.net/posts/2015-08-17-alex-happy-startcodes.html)
* [Calling Python libraries from Haskell](https://john-millikin.com/articles/ride-the-snake/)
* [Erasing "expected" messages in Parsec](http://jaspervdj.be/posts/2015-09-02-erasing-parsec-expected-messages.html)
* [bound](http://hackage.haskell.org/package/bound)
* [Write Yourself a Scheme in 48 Hours](http://en.wikibooks.org/wiki/Write_Yourself_a_Scheme_in_48_Hours) [[ja](https://ja.wikibooks.org/wiki/48%E6%99%82%E9%96%93%E3%81%A7Scheme%E3%82%92%E6%9B%B8%E3%81%93%E3%81%86)]
* [Write You a Haskell](http://dev.stephendiehl.com/fun/)
* [The Implementation of Functional Programming Languages](http://research.microsoft.com/en-us/um/people/simonpj/papers/slpj-book-1987/)
* [A Tutorial Implementation of a Dependently Typed Lambda Calculus](http://www.andres-loeh.de/LambdaPi/)
* [Introduction to PEG](http://www.slideshare.net/kmizushima/introduction-to-peg)
* [ビジュアル構文解析](http://www.slideshare.net/ichikaz3/ss-11400787)
* [Two kinds of backtracking](http://gelisam.blogspot.ca/2015/09/two-kinds-of-backtracking.html)
* [8章:関数型パーサ](http://www.slideshare.net/RuiccRail/programming-haskell-chapter8)
* [The megaparsec package](https://hackage.haskell.org/package/megaparsec)
* [Simple Monadic Parser in Haskell](http://michal.muskala.eu/2015/09/23/simple-monadic-parser-in-haskell.html)

##Extensible Effects
* [extensible-effects](https://hackage.haskell.org/package/extensible-effects)
* [Extensible Effects: an alternative to Monad Transformers](http://okmij.org/ftp/Haskell/extensible/)
* [suhailshergill/extensible-effects](https://github.com/suhailshergill/extensible-effects)
* [Extensible Effects](http://www.cs.indiana.edu/~sabry/papers/exteff.pdf)
* [Are extensible effects a complete replacement for mtl?](http://www.reddit.com/r/haskell/comments/387ex0/are_extensible_effects_a_complete_replacement_for/crt1pzm)
* [24 Days of Hackage: extensible-effects](https://ocharles.org.uk/blog/posts/2013-12-04-24-days-of-hackage-extensible-effects.html)
* [effin](https://hackage.haskell.org/package/effin)
* [The effect-handlers package](https://hackage.haskell.org/package/effect-handlers)
