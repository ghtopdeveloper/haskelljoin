* [The rebase package](http://hackage.haskell.org/package/rebase)
* [nikita-volkov/rerebase](https://github.com/nikita-volkov/rerebase)
* [Base で定義されている演算子の一覧](http://hackage.haskell.org/package/acme-operators/docs/Acme-Operators-Base.html)
* [The base-prelude package](https://hackage.haskell.org/package/base-prelude)
* [Foundation](http://tab.snarc.org/posts/haskell/2016-09-09-foundation.html)
* [順列列挙関数（素朴な実装）](http://qiita.com/nobsun/items/babd28fe81ba3b9f304f)
* [SamuelSchlesinger/Gaia](https://github.com/SamuelSchlesinger/Gaia) - An experiment in functional interface design

## 型
* [What is the difference between an Algebraic Data Type and an Abstract Data Type?](http://www.reddit.com/r/haskell/comments/38grqx/what_is_the_difference_between_an_algebraic_data/)
* [Either and (,) in Haskell are not arbitrary](http://bitemyapp.com/posts/2015-10-19-either-is-not-arbitrary.html)
* [Why sum and product types?](http://charlieharvey.org.uk/page/sum_and_product_types)
* [Types Don't Lie, But They Won't Reveal Everything](http://www.cli-nerd.com/2016/01/18/types-dont-lie-but-they-dont-reveal-everything.html)
* [Unit型の何が偉大なのか説明してみる](http://qiita.com/alucky0707/items/a677e5c9850aa765dd55)
* [Add a type parameter! One 'simple' design change, a panoply of outcomes](https://www.youtube.com/watch?v=BHjIl81HgfE)
* [The 6 types of Haskell users](http://rickdzekman.com/thoughts/the-6-types-of-haskell-users/)
* [Learning Haskell by Type (Signatures)](http://holger-peters.de/haskell-by-types.html)
* [ラムダ計算で代数的データ型を表現する方法](http://d.hatena.ne.jp/syamino/20120524/p1)
* [Associated Types and Haskell](http://amixtureofmusings.com/2016/05/19/associated-types-and-haskell/)
* [Better Data Types a la Carte](http://reasonablypolymorphic.com/blog/better-data-types-a-la-carte)
* [Sean Seefried - The Joy of Refactoring with Strong, Static Types](https://www.youtube.com/watch?v=_K6UAq4hjAs)
* [USING TYPES EFFECTIVELY](http://www.elbeno.com/presentations/using-types-effectively/presentation.html#/sec-title-slide)
* [Poop deprecation and shitty code](http://cs-syd.eu/posts/2016-08-28-poop-deprecation.html)
* [Maybe](http://qiita.com/knknkn1162/items/48427aee35bd5892c61d)
* [Pattern Synonyms](https://kseo.github.io/posts/2016-12-22-pattern-synonyms.html)
* [YOW! Lambda Jam 2016 Conor McBride - What are Types for, or are they only Against? - YouTube](https://www.youtube.com/watch?v=3U3lV5VPmOU&feature=share)
* [【Haskell】 言葉の定義まとめ（型クラス、型コンストラクタ、値コンストラクタ、型引数など） - takafumi blog](http://takafumi-s.hatenablog.com/entry/2015/09/25/123335)
* [Haskell による型安全プログラミングの実装例(和暦) - Qiita](http://qiita.com/algas/items/9e63f7a99303d27a6c03)
* [why-types/why-types.pdf at master · skaslev/why-types](https://github.com/skaslev/why-types/blob/master/why-types.pdf)
* [These, Align, and Crosswalk](http://teh.id.au/posts/2017/03/29/these-align-crosswalk/index.html)
* [Maybe? Use a type parameter!](http://www.parsonsmatt.org/2017/04/08/maybe_use_a_type_parameter.html)

### 代数的データ型
代数的データ型とは"足し算"と"掛け算"が出来るような型のこと。"足し算"と"掛け算"はそれぞれ**直和**, **直積** と呼ばれる。

```hs
-- 直和
type a + b = Either a b

-- 直積
type a * b = (a, b)
```

* [The algebra (and calculus!) of algebraic data types](https://codewords.recurse.com/issues/three/algebra-and-calculus-of-algebraic-data-types)
* [The Algebra of Programming in Haskell](http://www.cs.ox.ac.uk/research/pdt/ap/dgp/workshop2004/oliveira.pdf)
* [The Algebra of Algebraic Data Types, Part 1](http://chris-taylor.github.io/blog/2013/02/10/the-algebra-of-algebraic-data-types/)
* [Why are ADTs necessary?](http://www.reddit.com/r/haskell/comments/2z1n16/why_are_adts_necessary/)
* [Algebraic Data Types Demystified](http://blog.haskellformac.com/blog/algebraic-data-types-demystified)
* [Haskell Diary #2 - Algebra of Data Types](http://akashagrawal.me/haskell-diary-2-algebraic-data-types/)
* [Overcoming Boolean blindness with Evidence](http://cs-syd.eu/posts/2016-07-24-overcoming-boolean-blindness-evidence.html)
* [代数的データ型のデータのとりうる数を微分すると１穴空きデータ型の数になる話 - Qiita](http://qiita.com/mittyantest/items/f8783834e6bb48baf2c8)

### Codata
* [Codata](http://types2004.lri.fr/SLIDES/altenkirch.pdf)
* [Data and Codata](http://blog.sigfpe.com/2007/07/data-and-codata.html)

### Zipper
* [zipper](https://hackage.haskell.org/package/zipper)
* [Zippers - LYAH](http://learnyouahaskell.com/zippers)
* [データ型の微分](http://ja.wikibooks.org/wiki/Haskell/Zippers#.E3.83.87.E3.83.BC.E3.82.BF.E5.9E.8B.E3.81.AE.E5.BE.AE.E5.88.86)
* [Zippers, Part 2: Zippers as Derivatives](https://pavpanchekha.com/blog/zippers/derivative.html)
* [Scrap Your Zippers](http://michaeldadams.org/papers/scrap_your_zippers/ScrapYourZippers-2010.pdf)
* [syz](https://hackage.haskell.org/package/syz)
* [Zipper関連のパッケージ](http://d.hatena.ne.jp/debug-ito/20161016/1476587232)

##関数
* [A simple Haskell function](http://neilmitchell.blogspot.jp/2016/01/a-simple-haskell-function.html)
* [Composing bijections, surjections, and injections](https://gist.github.com/rampion/f20ffd6386269e6f7e41fae15d208e12)
* [Eastman maximal comma-free codes in Haskell](https://byorgey.wordpress.com/2016/07/07/eastman-maximal-comma-free-codes-in-haskell/)
* [Descriptive Variable Names: A Code Smell](http://degoes.net/articles/insufficiently-polymorphic)
* [map関数](http://qiita.com/knknkn1162/items/92de8dd250ff94cd86f1)

### パターンマッチ
* [Pattern matching](http://mbps.hatenablog.com/entry/2014/10/04/010000)
* [PATTERN MATCHING: WOT'S... UH THE DEAL?](http://www.stackbuilders.com/news/pattern-matching-wot-s-uh-the-deal)
* [Pattern and Guard Extensions](https://www.fpcomplete.com/school/to-infinity-and-beyond/pick-of-the-week/guide-to-ghc-extensions/pattern-and-guard-extensions)
* [Haskell で条件分岐](http://qiita.com/rooooomania/items/1623e5b981a30fbc8427)
* [コピペしてすぐ確認できるHaskellの条件分岐](http://qiita.com/nejimakidori/items/f6aedce6308ce5e32914)

###多変数関数とカリー化
* [Curry](https://ro-che.info/ccc/10)
* [Loop School - Curring](http://school.looprecur.com/?video=122330958)
* [Haskell Functions Take One Argument](http://tonymorris.github.io/blog/posts/haskell-functions-take-one-argument/)
* [A taste of Curry](https://jeltsch.wordpress.com/2013/04/27/a-taste-of-curry/)

```haskell
curry :: ((a, b) -> c) -> a -> b -> c
uncurry :: (a -> b -> c) -> (a, b) -> c
```

> Haskell 初心者は括弧ばかりの Lisp のようなコードを書く。中級者になると、($) が多くなる。上級者(言い過ぎか？)になると、($) が消えて、(.) が多くなる。

出典: [関数合成の妙技](http://d.hatena.ne.jp/kazu-yamamoto/20100702/1278036842)

### ポイントフリー
必要のないところでポイントワイズに書く必要はないが、あまりポイントフリーに拘りすぎないのも大事

* [ポイントフリースタイル入門](http://d.hatena.ne.jp/melpon/20111031/1320024473)
* [Haskellのフクロウ ((.)$(.))](http://uid0130.blogspot.jp/2014/11/haskell_17.html)
* [Blunt](https://blunt.herokuapp.com/)
  * [pointfree](https://hackage.haskell.org/package/pointfree)
* ["Point-Free or Die: Tacit Programming in Haskell and Beyond" by Amar Shah](https://www.youtube.com/watch?v=seVSlKazsNk)

### 遅延評価
* [Schrödinger's cat](https://ro-che.info/ccc/4)
* [Résumé](https://ro-che.info/ccc/11)
* [正格評価と遅延評価（基本編）](http://qiita.com/ruicc/items/07143c9e78c697227706)
* [正格評価と遅延評価（詳細編）](http://qiita.com/ruicc/items/31a269f93404268d80d7)
* [takenobu-hs/lazy_evaluation](https://github.com/takenobu-hs/lazy_evaluation)
* [なぜHaskellでタライ回しが速いのか、あるいは遅延評価とSTG](http://qiita.com/ruicc/items/b8b3c61a12baa1af3c69)

> One very interesting comparison is that lazy evaluation is to the CPU what garbage collection is to memory.

出典: <http://scott.sauyet.com/Javascript/Talk/2014/01/FuncProgTalk/#slide-40>

**遅延評価を利用したメモ化の実装例**

```haskell
fibs :: [Integer]
fibs = map fib [0..]

fib :: Int -> Integer
fib 0 = 1
fib 1 = 1
fib n = fibs !! (n-1) + fibs !! (n-2)
```

参考: [Can someone explain the concept behind Haskell's memoization?](http://programmers.stackexchange.com/questions/220746/can-someone-explain-the-concept-behind-haskells-memoization)

* [The Incomplete Guide to Lazy Evaluation (in Haskell)](https://hackhands.com/guide-lazy-evaluation-haskell/)
* [If Haskell were strict, what would the laziness be like?](http://nikita-volkov.github.io/if-haskell-were-strict/)
* [How to force a list](https://ro-che.info/articles/2015-05-28-force-list)
* [Thinking with Laziness](http://begriffs.com/posts/2015-06-17-thinking-with-laziness.html)
* [How Laziness Works](http://two-wrongs.com/how-laziness-works)
* [Haskell memoization](http://lukahorvat.github.io/programming/2014/11/18/haskell-memoization/)
* [Haskellでメモ化を行うもう一つの方法](http://d.hatena.ne.jp/tanakh/20100411)
* [Kwang's Haskell Blog - Memoization in Haskell](https://kseo.github.io//posts/2017-01-14-memoization-in-hasekll.html)

### 部分関数
* [Partial Function Considered Harmful](http://tanakh.jp/posts/2011-12-25-partial-function-considered-harmful.html)
* <https://twitter.com/GabrielG439/status/671803691591077888>
* [24 days of Hackage, 2015: day 16: safe; what is safety anyway?](http://conscientiousprogrammer.com/blog/2015/12/16/24-days-of-hackage-2015-day-16-safe-what-is-safety-anyway/)
* [部分関数をどう扱うか(spoonの紹介)](http://qiita.com/techno-tanoC/items/1b725713cd01bdf83b40)
* [The spoon package](https://hackage.haskell.org/package/spoon)

---

* [Generalizing function composition](http://jaspervdj.be/posts/2014-10-17-generalizing-function-composition.html)
* [Haskell Symposium 2012. Koen Claessen: Shrinking and showing functions](https://www.youtube.com/watch?v=CH8UQJiv9Q4)
* [Making a fast curry Push/enter vs eval/apply for higher-order languages](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.134.9317&rep=rep1&type=pdf)
* [A Pragmatic Case for Static Typing with Brian Hurt](https://vimeo.com/72870631)
* [On stateless software design: what is state ?](http://www.leonmergen.com/code/2015/12/04/on-stateless-software-design-what-is-state.html)
* [Does Haskell make promises it can't keep? or The big problem with wrapping numeric types](https://gist.github.com/tdoris/de36d2306edc5d6e9e7d#file-promises-md)
