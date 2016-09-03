* [DataHaskell](https://datahaskell.github.io/)
* [random-fu](https://hackage.haskell.org/package/random-fu)
* [mikeizbicki/HLearn](https://github.com/mikeizbicki/HLearn/)
  * [Haskellの機械学習ライブラリHLearn](http://qiita.com/nebutalab/items/680203ff3d84cde7c8db)
* [bmsherman/haskell-matlab](https://github.com/bmsherman/haskell-matlab)
* [HaskellR](http://tweag.github.io/HaskellR/)
  * [Programming R at native speed using Haskell](http://www.tweag.io/blog/programming-r-at-native-speed-using-haskell)
  * [How to include R plots and diagrams in blog posts](http://www.corentindupont.info/blog/posts/Programming/2015-09-14-diagrams.html)
* [QLearn: A Haskell library for iterative Q-learning.](http://poincare.github.io/QLearn/)
* [Automatic Propagation of Uncertainty with AD](https://blog.jle.im/entry/automatic-propagation-of-uncertainty-with-ad.html)
* [Kalman filters and functional programming](http://www.johndcook.com/blog/2016/07/14/kalman-filters-and-functional-programming/)
* [aneksteind/hext](https://github.com/aneksteind/hext)
* [Demo of IHaskell Notebook](http://begriffs.com/posts/2016-01-20-ihaskell-notebook.html)
* [bitemyapp/bloodhound](https://github.com/bitemyapp/bloodhound) - Haskell Elasticsearch client and query DSL
* [IHaskell Online: Help Choose Demo Code Snippets!](http://www.reddit.com/r/haskell/comments/37uqqk/ihaskell_online_help_choose_demo_code_snippets/)
* [関数型言語Haskellを用いた役割指向エージェントベースシミュレーションシステムのプロトタイプ開発](http://repo.lib.hosei.ac.jp/handle/10114/11016)
* [Install IHaskell on Ubuntu 14.04 with Stack](http://remusao.github.io/install-ihaskell-on-ubuntu-1404-with-stack.html)
* [プログラミングのための確率統計 in Haskell](http://note.golden-lucky.net/2010/12/1-2-3-4-5-6-16-16-16-16-16-16-246-135.html)
* [HuwCampbell/grenade](https://github.com/HuwCampbell/grenade)
* [FRP & RNN](http://imgur.com/a/mWseu)
* [DeepLearning(1): まずは順伝播(上)](http://qiita.com/eijian/items/06b1ba1276d1bfd77b93)
* [Get a Brain](http://www-cs-students.stanford.edu/~blynn//haskell/brain.html)

## 確率論的プログラミング
* Church
  * [Church: a language for generative models](https://cocolab.stanford.edu/papers/GoodmanEtAl2008-UncertaintyInArtificialIntelligence.pdf)
  * [Probabilistic Models of Cognition](https://probmods.org/)

```hs
type Probability = Double
newtype Dist a = D {unD :: [(a,Probability)]}

instance Monad Dist where
  return x = D [(x,1)]
  (D d) >>= f = D [(y,q*p) | (x,p) <- d, (y,q) <- unD (f x)]
```
[FUNCTIONAL PEARLS: Probabilistic Functional Programming in Haskell](https://web.engr.oregonstate.edu/~erwig/papers/PFP_JFP06.pdf)

* [Learning Probabilistic Programs](http://arxiv.org/abs/1407.2646)
* [A Probabilistic Functional Programming Library for Haskell](https://web.engr.oregonstate.edu/~erwig/pfp/)
* [A New Approach to Probabilistic Programming Inference](http://www.robots.ox.ac.uk/~fwood/assets/pdf/Wood-AISTATS-2014.pdf)
* [FMFMFMF: Free Monads For Making Fast Models, Functionally.](http://statusfailed.com/blog/2015/09/04/free-monads-for-making-fast-models.html)
* [Practical Probabilistic Programming with Monads](https://www.youtube.com/watch?v=hI0ajVy2xEk)
* [Practical probabilistic programming with monads](http://dl.acm.org/citation.cfm?id=2804317)
* [Probabilistic Programming & Bayesian Methods for Hackers](http://camdavidsonpilon.github.io/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/)
* [Probabilistic inference by program transformation in Hakaru (system description)](http://homes.soic.indiana.edu/ccshan/rational/system.pdf)
* [Simplifying Probabilistic Programs Using Computer Algebra](http://www.cs.indiana.edu/ftp/techreports/TR719.pdf)
* [Abstract Binding Trees in Hakaru](http://winterkoninkje.dreamwidth.org/103978.html)
* [Encoding Statistical Independence, Statically](http://jtobin.ca/encoding-independence-statically)
* [Stochastic Lambda Calculus and Monads of Probability Distributions](https://www.cs.tufts.edu/~nr/pubs/pmonad.pdf)
* [Bayesian Optimization for Probabilistic Programs](http://www.blackboxworkshop.org/pdf/rainforth2015BOPP.pdf)
* [Practical Probabilistic Programming with Monads](http://mlg.eng.cam.ac.uk/pub/pdf/SciGhaGor15.pdf)
* [A Categorical Basis for Conditional Probability](http://www.cs.ru.nl/B.Jacobs/PAPERS/cat-prob-th.pdf)
* [BAli-Phy](http://www.bali-phy.org/)
* [Stanで統計モデリングを学ぶ(1): まずはStanの使い方のおさらいから](http://tjo.hatenablog.com/entry/2014/01/27/235048)
* [Anglican](http://www.robots.ox.ac.uk/~fwood/anglican/)

## Hakaru
* [hakaru-dev/hakaru](https://github.com/hakaru-dev/hakaru)
* [hakaru: A probabilistic programming embedded DSL](https://hackage.haskell.org/package/hakaru)
* [Hakaru: An embedded probabilistic programming language for Haskell.](http://indiana.edu/~ppaml/)

```hs
heads = Just (toDyn (Discrete True))

prog :: Measure Double
prog = do
   bias <- unconditioned (beta 1 1)
   replicateM 10 $ conditioned (bern bias)
   return bias

sample prog (replicate 10 heads)
```

## Categorical Probability Theory
* [Categorical Probability Theory](https://arxiv.org/abs/1406.6030)
* [Giry monad](https://ncatlab.org/nlab/show/Giry+monad)
* [A CATEGORICAL FOUNDATION FOR BAYESIAN PROBABILITY](https://arxiv.org/pdf/1205.1488.pdf)
* [A Type Theory for Probabilistic and Bayesian Reasoning](https://arxiv.org/pdf/1511.09230v1.pdf)
