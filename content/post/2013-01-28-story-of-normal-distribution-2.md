---
title: 正态分布的前世今生(下)
date: '2013-01-28T22:45:44+00:00'
author: rickjin
categories:
  - 经典理论
tags:
  - 历史
  - 正态分布
  - 经典理论
slug: story-of-normal-distribution-2
---

**6. 开疆拓土，正态分布的进一步发展**

19世纪初，随着拉普拉斯中心极限定理的建立与高斯正态误差理论的问世，正态分布开始崭露头角，逐步在近代概率论和数理统计学中大放异彩。在概率论中，由于拉普拉斯的推动，中心极限定理发展成为现代概率论的一块基石。而在数理统计学中，在高斯的大力提倡之下，正态分布开始逐步畅行于天下。

**6.1 论剑中心极限定理**

先来说说正态分布在概率论中的地位，这个主要是由于中心极限定理的影响。 1776 年，拉普拉斯开始考虑一个天文学中的彗星轨道的倾角的计算问题，最终的问题涉及独立随机变量求和的概率计算，也就是计算如下的概率值
  
$$ S\_n = X\_1 + X\_2 + \cdots + X\_n $$
  
$$P(a < S_n < b) = ? $$

在这个问题的处理上，拉普拉斯充分展示了其深厚的数学分析功底和高超的概率计算技巧，他首次引入了特征函数(也就是对概率密度函数做傅立叶变换)来处理概率分布的神妙方法，而这一方法经过几代概率学家的发展，在现代概率论里面占有极其重要的位置。基于这一分析方法，拉普拉斯通过近似计算，在他的1812年发表的名著《概率分析理论》中给出了中心极限定理的一般描述：

**定理：[拉普拉斯, 1812]**  $ e\_i (i=1, \cdots n)$ 为独立同分布的测量误差，具有均值$\mu$ 和方差 $\sigma^2$。如果 $\lambda\_1, \cdots, \lambda_2$ 为常数， $a>0$, 则有
  
$$ \displaystyle P\left(\left|\sum\_{i=1}^n \lambda\_i(e_i &#8211; \mu)\right|
  
\le a \sqrt{\sum\_{i=1}^n \lambda\_i^2}\right)
  
\approx \frac{2}{\sqrt{2\pi}\sigma} \int_0^a e^{-\frac{x^2}{2\sigma^2}} dx . $$

这已经是比棣莫弗-拉普拉斯中心极限定理更加深刻的一个结论了，理科专业的本科生学习《概率论与数理统计》这门课程的时候，通常学习的中心极限定理的一般形式如下：

**[林德伯格-列维 中心极限定理]** 设$X\_1,\cdots, X\_n$ 独立同分布，且具有有限的均值 $\mu$ 和方差 $\sigma^2$ ，则在 $n \rightarrow \infty$ 时,有
  
$$ \displaystyle \frac{\sqrt{n}(\overline{X} &#8211; \mu)}{\sigma} \rightarrow N(0,1) .$$

多么奇妙的性质，随意的一个概率分布中生成的随机变量，在序列和(或者等价的求算术平均)的操作之下，表现出如此一致的行为，统一的规约到正态分布。

<p style="text-align: center">
  <a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/central_limit_theorem/" rel="attachment wp-att-7076"><img class="aligncenter size-full wp-image-7076" alt="central_limit_theorem" src="https://cos.name/wp-content/uploads/2013/01/central_limit_theorem.jpg" width="548" height="185" srcset="https://cos.name/wp-content/uploads/2013/01/central_limit_theorem.jpg 548w, https://cos.name/wp-content/uploads/2013/01/central_limit_theorem-300x101.jpg 300w, https://cos.name/wp-content/uploads/2013/01/central_limit_theorem-500x168.jpg 500w" sizes="(max-width: 548px) 100vw, 548px" /></a><strong>中心极限定理</strong>
</p>

概率学家们进一步的研究结果更加令人惊讶，序列求和最终要导出正态分布的条件并不需要这么苛刻，即便 $X\_1,\cdots, X\_n$ 并不独立，也不具有相同的概率分布形式，很多时候他们求和的最终的归宿仍然是正态分布。一切的纷繁芜杂都在神秘的正态曲线下被消解，这不禁令人浮想联翩。中心极限定理恐怕是概率论中最具有宗教神秘色彩的定理，如果有一位牧师拿着一本圣经向我证明上帝的存在，我是丝毫不会买账；可是如果他向我展示中心极限定理并且声称那是神迹，我可能会有点犹豫，从而乐意倾听他的布道。如果我能坐着时光机穿越到一个原始部落中，我也一定带上中心极限定理，并劝说部落的酋长把正态分布作为他们的图腾。

<!--more-->中心极限定理虽然表述形式简洁，但是严格证明它却非常困难。中心极限定理就像一张大蜘蛛网，棣莫弗和拉普拉斯编织了它的雏形，可是这张网上漏洞太多，一个多世纪来，数学家们就像蜘蛛一样前赴后继，努力想把所有的漏洞都补上。在19世纪，泊松 (Siméon Denis Poisson, 1781-1840)、狄利克莱(Gustav Lejeune Dirichlet, 1805-1859)、柯西(Augustin-Louis Cauchy, 1789-1857)、贝塞尔(Friedrich Bessel, 1784-1846)这些大蜘蛛都曾经试图对把这张网上的漏洞补上。从现代概率论的角度来看，整个19世纪的经典概率理论并没有能输出一个一般意义下严格的证明。而真正把漏洞补上的是来自俄罗斯的几位蜘蛛侠：切比雪夫(Pafnuty Chebyshev, 1821-1894)、马尔可夫(Andrey Andreyevich Markov, 1856-1922)和李雅普诺夫(Aleksandr Mikhailovich Lyapunov, 1857-1918)。俄罗斯是一个具有优秀的数学传统的民族，产生过几位顶尖的的数学家，在现代概率论的发展中，俄罗斯的圣彼得堡学派可以算是顶了半边天。把漏洞补上的严格方案的雏形是从切比雪夫 1887年的工作开始的，不过切比雪夫的证明存在一些漏洞。马尔可夫和李雅普诺夫都是切比雪夫的学生，马尔科夫沿着老师的基于矩法的思路在蜘蛛网上辛勤编织，但洞还是补得不够严实；李雅普诺夫不像马尔可夫那样深受老师的影响，他沿着拉普拉斯当年提出的基于特征函数的思路，于1901年给出了一个补洞的方法，切比雪夫对这个方法大加赞赏，李雅普诺夫的证明被认为是第一个在一般条件下的严格证明；而马尔科夫也不甘示弱，在 1913年基于矩法也把洞给补严实了。

&nbsp;

<p style="text-align: center">
  <a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/clt_proof/" rel="attachment wp-att-7080"><img class="aligncenter size-full wp-image-7080" alt="clt_proof" src="https://cos.name/wp-content/uploads/2013/01/clt_proof.jpg" width="601" height="126" srcset="https://cos.name/wp-content/uploads/2013/01/clt_proof.jpg 601w, https://cos.name/wp-content/uploads/2013/01/clt_proof-300x62.jpg 300w, https://cos.name/wp-content/uploads/2013/01/clt_proof-500x104.jpg 500w" sizes="(max-width: 601px) 100vw, 601px" /></a><strong>华山论剑</strong>
</p>

20世纪初期到中期，中心极限定理的研究几乎吸引了所有的概率学家，这个定理俨然成为了概率论的明珠，成为了各大概率论武林高手华山论剑的场所。不知道大家对中心极限定理中的“中心”一词如何理解，许多人都认为“中心”这个词描述的是这个定理的行为：以正态分布为中心。这个解释看起来确实合情合理，不过并不符合该定理被冠名的历史。事实上，20世纪初概率学家大都称呼该定理为极限定理(Limit Theorem)，由于该定理在概率论中处于如此重要的中心位置，如此之多的概率学武林高手为它魂牵梦绕，于是数学家波利亚于1920年在该定理前面冠以“中心”一词，由此后续人们都称之为中心极限定理。

数学家们总是极其严谨苛刻的，给定了一个条件下严格证明了中心极限定理。数学家就开始探寻中心极限定理成立的各种条件，询问这个条件是否充分必要条件，并且进一步追问序列和在该条件下以什么样的速度收敛到正态分布。1922年林德伯格(Jarl Waldemar Lindeberg, 1876-1932) 基于一个比较宽泛容易满足的条件，给中心极限定理提出了一个很容易理解的初等证明，这个条件我们现在称之为林德伯格条件。然后概率学家费勒 (William Feller, 1906-1970) 和列维就开始追问林德伯格 条件是充分必要的吗？基于林德伯格的工作， 费勒和列维都于 1935 年独立的得到了中心极限定理成立的充分必要条件，这个条件可以用直观的非数学语言描述如下：

**[中心极限定理充要条件]** 假设独立随机变量序列 $X\_i$ 的中值为0, 要使序列和 $\displaystyle S=\sum\_{i=1}^n
  
X_i$ 的分布密度函数逼近正态分布，以下条件是充分必要的

  * 如果 $X\_i$相对于序列和$S$的散布(也就是标准差)是不可忽略的，则 $X\_i$ 的分布必须接近正态分布
  * 对于所有可忽略的 $X_i$, 取绝对值最大的那一项，这个绝对值相对于序列和也是可忽略的

事实上这个充分必要条件发现的优先权，费勒和列维之间还着实出现了一些争论，当然他们俩都是独立的几乎在同一时间解决了这个问题。在列维证明这个充分必要条件的过程中，列维发现了正态分布的一个有趣的性质：我们在数理统计中都学过，如果两个独立随机变量 $X,Y$ 具有正态分布，则$S=X+Y$ 也具有正态分布；奇妙的是这个定理的逆定理也成立：

**[正态分布的血统] **如果 $X,Y$ 是独立的随机变量，且 $S=X+Y$ 是正态分布，那么 $X,Y$ 也是正态分布。

正态分布真是很奇妙，就像蚯蚓一样具有再生的性质，你把它一刀两断，它生成两个正态分布；或者说正态分布具有极其高贵的优良血统，正态分布的组成成分中只能包含正态分布，而不可能含有其它杂质。一流的数学家都是接近上帝的人，善于猜测上帝的意图； 1928 年 列维就猜到了这个定理，并在1935年使用这个定理对中心极限定理的充分必要条件作了证明。有意思的是列维却无法证明正态分布的这个看上去极其简单的再生性质，所以他的证明多少让人觉得有些瑕疵。不过列维的救星很快就降临了，1936 年概率学家克拉美(Harald Cramér, 1893-1985)证明列维的猜想完全正确。

中心极限定理成为了现代概率论中首屈一指的定理，事实上中心极限定理在现代概率论里面已经不是指一个定理，而是指一系列相关的定理。统计学家们也基于该定理不断的完善拉普拉斯提出的元误差理论，并据此解释为何世界上正态分布如此常见。而中心极限定理同时成为了现代统计学中大样本理论的基础。

**6.2 进军近代统计学**

花开两朵，各表一枝。上面说了正态分布在概率论中的发展，现在来看看正态分布在数理统计学中发展的故事。这个故事的领衔主演是凯特勒(Adolphe Quetelet, 1796-1874)和高尔顿 (Francis Galton, 1822-1911)。

<p style="text-align: center">
  <strong><a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/galton_quetelet/" rel="attachment wp-att-7048"><img class="aligncenter size-full wp-image-7048" alt="galton_quetelet" src="https://cos.name/wp-content/uploads/2013/01/galton_quetelet.jpg" width="364" height="207" srcset="https://cos.name/wp-content/uploads/2013/01/galton_quetelet.jpg 364w, https://cos.name/wp-content/uploads/2013/01/galton_quetelet-300x170.jpg 300w" sizes="(max-width: 364px) 100vw, 364px" /></a>凯特勒和高尔顿</strong>
</p>

由于高斯的工作，正态分布在误差分析中迅速确定了自己的地位。有了这么好的工具，我们可能拍脑袋就认为，正态分布很快就被人们用来分析其它的数据，然而事实却出乎我们的意料，正态分布进入社会领域和自然科学领域，可是经过一番周折的。

首先我要告诉大家一个事实：误差分析和统计学是风马牛不相及的两个学科；当然这个事实存在的时间是19世纪初之前。统计学的产生最初是与“编制国情报告”有关，主要服务于政府部门。统计学面对的是统计数据，是对多个不同对象的测量；而误差分析研究的是观测数据，是对同一个对象的多次测量。因此观测数据和统计数据在当时被认为是两种不同行为获取得到的数据，适用于观测数据的规律未必适用于统计数据。 19世纪的统计数据分析处于一个很落后的状态，和概率论没有多少结合。概率论的产生主要和赌博相关，发展过程中与误差分析紧密联系，而与当时的统计学交集非常小。将统计学与概率论真正结合起来推动数理统计学发展的便是我们的统计学巨星凯特勒。

凯特勒这名字或许不如其它数学家那么响亮，估计很多人不熟悉，所以有必要介绍一下。 凯特勒是比利时人，数学博士毕业，年轻的时候曾追随拉普拉斯学习过概率论。此人学识渊博，涉猎广泛，脑门上的桂冠包括统计学家、数学家、天文学家、社会学家、国际统计会议之父、近代统计学之父、数理统计学派创始人。 凯特勒 的最大的贡献就是将法国的古典概率理论引入统计学，用纯数学的方法对社会现象进行研究。

1831年，凯特勒参与主持新建比利时统计总局的工作。他开始从事有关人口问题的统计学研究。在这种研究中，凯特勒发现,以往被人们认为杂乱无章的、偶然性占统治地位的社会现象，如同自然现象一样也具有一定的规律性。 凯特勒 搜集了大量关于人体生理测量的数据，如体重、身高与胸围等，并使用概率统计方法来对数据进行数据分析。但是当时的统计分析方法遭到了社会学家的质疑，社会学家们的反对意见主要在于：社会问题与科学实验不同，其数据一般由观察得到，无法控制且经常不了解其异质因素，这样数据的同质性连带其分析结果往往就有了问题，于是社会统计工作者就面临一个如何判断数据同质性的问题。凯特勒大胆地提出：

<p style="text-align: center">
  <strong><a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/normal_fitness/" rel="attachment wp-att-7063"><img class="aligncenter  wp-image-7063" alt="normal_fitness" src="https://cos.name/wp-content/uploads/2013/01/normal_fitness.jpg" width="326" height="276" srcset="https://cos.name/wp-content/uploads/2013/01/normal_fitness.jpg 408w, https://cos.name/wp-content/uploads/2013/01/normal_fitness-300x253.jpg 300w, https://cos.name/wp-content/uploads/2013/01/normal_fitness-354x300.jpg 354w" sizes="(max-width: 326px) 100vw, 326px" /></a>把一批数据是否能很好地拟合正态分布，作为判断该批数据同质的标准。</strong>
</p>

凯特勒提出了一个使用正态曲线拟合数据的方法，并广泛的使用正态分布去拟合各种类型的数据。由此， 凯特勒为正态分布的应用拓展了广阔的舞台。正态分布如同一把屠龙刀，在凯特勒 的带领下，学者们挥舞着这把宝刀在各个领域披荆斩棘，攻陷了人口、领土、政治、农业、工业、商业、道德等社会领域，并进一步攻占天文学、数学、物理学、生物学、社会统计学及气象学等自然科学领域。

正态分布的下一个推动力来自生物学家高尔顿，当正态分布与生物学联姻时，近代统计学迎来了一次大发展。高尔顿是生物统计学派的奠基人，他的表哥达尔文的巨著《物种起源》问世以后，触动他用统计方法研究遗传进化问题。受凯特勒的启发，他对正态分布怀有浓厚的兴趣，开始使用正态分布去拟合人的身高、胸围、以至考试成绩等各类数据，发现正态分布拟合得非常好。他因此相信正态曲线是适用于无数情况的一般法则。

然而，对高尔顿而言，这个无处不在的正态性给他带来一些困惑。他考察了亲子两代的身高数据，发现遵从同一的正态分布，遗传作为一个显著因素是如何发挥作用的？1877年，高尔顿设计了一个叫高尔顿钉板(quincunx, 或者Galton board)的装置，模拟正态分布的性质，用于解释遗传现象。

如下图中每一点表示钉在板上的一颗钉子，它们彼此的距离均相等。当小圆球向下降落过程中，碰到钉子后皆以 1/2 的概率向左或向右滚下。如果有n排钉子，则各槽内最终球的个数服从二项分布 $B(n,1/2)$, 当$n$ 较大的时候，接近正态分布。

<p style="text-align: center">
  <strong><a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/galton_quincunx/" rel="attachment wp-att-7051"><img class="aligncenter size-full wp-image-7051" alt="galton_quincunx" src="https://cos.name/wp-content/uploads/2013/01/galton_quincunx.jpg" width="569" height="347" srcset="https://cos.name/wp-content/uploads/2013/01/galton_quincunx.jpg 569w, https://cos.name/wp-content/uploads/2013/01/galton_quincunx-300x182.jpg 300w, https://cos.name/wp-content/uploads/2013/01/galton_quincunx-500x304.jpg 500w, https://cos.name/wp-content/uploads/2013/01/galton_quincunx-491x300.jpg 491w" sizes="(max-width: 569px) 100vw, 569px" /></a>高尔顿钉板</strong>
</p>

设想在此装置的中间某个地方 AB 设一个挡板把小球截住，小球将在AB处聚成正态曲线形状，如果挡板上有许多阀门，打开一些阀门，则在底部形成多个大小不一的正态分布，而最终的大正态分布正是这些小正态分布的混合。

<p style="text-align: center">
  <strong><a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/galton_quincunx3/" rel="attachment wp-att-7050"><img class="aligncenter size-full wp-image-7050" alt="galton_quincunx3" src="https://cos.name/wp-content/uploads/2013/01/galton_quincunx3.jpg" width="555" height="227" srcset="https://cos.name/wp-content/uploads/2013/01/galton_quincunx3.jpg 555w, https://cos.name/wp-content/uploads/2013/01/galton_quincunx3-300x122.jpg 300w, https://cos.name/wp-content/uploads/2013/01/galton_quincunx3-500x204.jpg 500w" sizes="(max-width: 555px) 100vw, 555px" /></a>高尔顿钉板解释遗传现象</strong>
</p>

高尔顿利用这个装置创造性的把正态分布的性质用于解释遗传现象。他解释说身高受到显著因素和其它较小因素的影响，每个因素的影响可以表达为一个正态分布。遗传作为一个显著因素，类似图中底部大小不一的正态分布中的比较大的正态分布，而多个大小不一正态分布累加之后其结果仍然得到一个正态分布。

高尔顿在研究身高的遗传效应的时候，同时发现一个奇特的现象：高个子父母的子女，其身高有低于其父母身高的趋势，而矮个子父母的子女，其身高有高于其父母的趋势，即有“回归”到普通人平均身高去的趋势，这也是“回归”一词最早的含义。高尔顿用二维正态分布去拟合父代和子代身高的数据，同时引进了回归直线、相关系数的概念，从而开创了回归分析这门技术。

可以说，高尔顿是用统计方法研究生物学的第一人，他用实际行动开拓了凯特勒的思想；为数理统计学的产生奠定了基础。无论是 凯特勒 还是高尔顿，他们的统计分析工作都是以正态分布为中心的，在他们的影响下，正态分布获得了普遍认可和广泛应用，甚至是被滥用，以至有些学者认为19世纪是正态分布在统计学中占统治地位的时代。

**6.3 数理统计三剑客**

最后，我们来到了20世纪，正态分布的命运如何呢？如果说19世纪是正态分布在统计学中独领风骚的话，20世纪则是数理统计学蓬勃发展、百花齐放的时代。 1901年，高尔顿和他的学生卡尔.皮尔逊(Karl Pearson, 1857-1936)、韦尔登(Walter Frank Raphael Weldon, 1860-1906) 创办《生物计量 (Biometrika)》杂志，成为生物统计学派的一面旗帜，引导了现代数理统计学的大发展。统计学的重心逐渐由欧洲大陆向英国转移，使英国在以后几十年数理统计学发展的黄金时代充当了领头羊。

在20世纪以前，统计学所处理的数据一般都是大量的、自然采集的，所用的方法以拉普拉斯中心极限定理为依据，总是归结到正态。到了19世纪末期，数据与正态拟合不好的情况也日渐为人们所注意：进入20世纪之后，人工试验条件下所得数据的统计分析问题，逐渐被人们所重视。由于试验数据量有限，那种依赖于近似正态分布的传统方法开始招致质疑，这促使人们研究这种情况下正确的统计方法问题。

在这个背景之下，统计学三大分布$\chi^2$分布、$t$分布、$F$分布逐步登上历史舞台。这三大分布现在的理科本科生都很熟悉。在历史上，这三个分布和来自英国的现代数理统计学的三大剑客有着密切的关系。

<p style="text-align: center">
  <a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/three-swords/" rel="attachment wp-att-7069"><img class="aligncenter size-full wp-image-7069" alt="three-swords" src="https://cos.name/wp-content/uploads/2013/01/three-swords.jpg" width="576" height="217" srcset="https://cos.name/wp-content/uploads/2013/01/three-swords.jpg 576w, https://cos.name/wp-content/uploads/2013/01/three-swords-300x113.jpg 300w, https://cos.name/wp-content/uploads/2013/01/three-swords-500x188.jpg 500w" sizes="(max-width: 576px) 100vw, 576px" /></a>数理统计三剑客
</p>

第一位剑客就是卡尔.皮尔逊，手中的宝剑就是$\chi^2$分布。 $\chi^2$ 分布这把宝剑最早的锻造者其实是物理学家麦克斯韦，他在推导空气分子的运动速度的分布的时候，发现分子速度在三个坐标轴上的分量是正态分布，而分子运动速度的平方$v^2$ 符合自由度为3 的$\chi^2$分布。麦克斯韦虽然造出了这把宝剑，但是真正把它挥舞得得心应手、游刃有余的是皮尔逊。在分布曲线和数据的拟合优度检验中，$\chi^2$分布可是一个利器，而皮尔逊的这个工作被认为是假设检验的开山之作。皮尔逊继承了高尔顿的衣钵，统计功力深厚，在19世纪末20世纪初很长的一段时间里，一直被数理统计武林人士尊为德高望重的第一大剑客。

第二位剑客是戈塞特(William Sealy Gosset, 1876-1937)，笔名是大家都熟悉的学生氏 (Student)，而他手中的宝剑是 $t$ 分布。戈塞特是化学、数学双学位，依靠自己的化学知识进酿酒厂工作，工作期间考虑酿酒配方实验中的统计学问题，追随卡尔.皮尔逊学习了一年的统计学，最终依靠自己的数学知识打造出了$t$分布这把利剑而青史留名。 1908年，戈塞特提出了正态样本中样本均值和标准差的比值的分布，并给出了应用上极其重要的第一个分布表。戈塞特在$t$ 分布的工作开创了小样本统计学的先河。

第三位剑客是费希尔(Ronald Aylmer Fisher, 1890-1962)，手持$F$分布这把宝剑，在一片荒芜中开拓出方差分析的肥沃土地。 $F$分布就是为了纪念费希尔而用他的名字首字母命名的。费希尔剑法飘逸，在三位剑客中当属费希尔的天赋最高，各种兵器的使用都得心应手。费希尔统计造诣极高，受高斯的启发，系统的创立了极大似然估计剑法，这套剑法现在被尊为统计学参数估计中的第一剑法。

费希尔还未出道，皮尔逊已经是统计学的武林盟主了，两人岁数相差了33岁，而戈塞特介于他们中间。三人在统计学擂台上难免切磋剑术。费希尔天赋极高，年少气盛；而皮尔逊为人强势，占着自己武林盟主的地位，难免固执己见，以大欺小；费希尔着实受了皮尔逊不少气。而戈塞特性格温和，经常在两位大侠之间调和。毕竟是长江后浪推前浪，一代新人换旧人，在众多擂台比试中，费希尔都技高一筹，而最终取代了皮尔逊成为数理统计学第一大剑客。

由于这三大剑客和统计三大分布的出现，正态分布在数理统计学中不再是一枝独秀，数理统计的领地基本上是被这三大分布抢走了半壁江山。不过这对正态分布而言并非坏事，我们细看这三大分布的数学细节: 假设独立随机变量 $X\_i \sim N(0,1), Y\_j \sim N(0,1) (i=1\cdots n, j=1\cdots m)$，则满足三大分布的随机变量可以如下构造出来

  * $ \displaystyle \chi\_n^2 = X\_1^2 + \cdots + X_n^2$
  * $ \displaystyle t = \frac{Y\_1}{\sqrt{\frac{X\_1^2 + \cdots + X_n^2}{n}}}$
  * $ \displaystyle F = \frac{\frac{X\_1^2 + \cdots + X\_n^2}{n}}{\frac{Y\_1^2 + \cdots + Y\_m^2}{m}} $

你看这三大分布哪一个不是正态分布的嫡系血脉，$\chi^2$、 $t$、$F$这三大分布最初都是从正态分布切入进行研究的。所以正态分布在19世纪是武则天，进入20世纪就学了慈禧太后，垂帘听政了。或者，换个角度说，一个好汉三个帮，正态分布如果是孤家寡人恐怕也难以雄霸天下，有了统计学三大分布作为开国先锋为它开疆拓土，正态分布真正成为傲世群雄的君王。

20世纪初，统计学这三大剑客成为了现代数理统计学的奠基人。以哥塞特为先驱，费希尔为主将，掀起了小样本理论的革命，事实上提升了正态分布在统计学中的地位。在数理统计学中，除了以正态分布为基础的小样本理论获得了空前的胜利，其它分布上都没有成功的案例，这不能不让人对正态分布刮目相看。在随后的发展中，相关回归分析、多元分析、方差分析、因子分析、布朗运动、高斯过程等等诸多概率统计分析方法陆续登上了历史舞台，而这些和正态分布密切相关的方法，成为推动现代统计学飞速发展的一个强大动力。

**7. 正态魅影**

_Everyone believes in it: experimentalists believing that it is a mathematical theorem, mathematicians believing that it is an empirical fact. _
  
_&#8212; Henri Poincaré_

如果说，充斥着偶然性的世界是一个纷乱的世界，那么，正态分布为这个纷乱的世界建立了一定的秩序，使得偶然性现象在数量上被计算和预测成为可能。杰恩斯在《概率论沉思录》中提出了两个问题

  1. 为什么正态分布被如此广泛的使用？
  2. 为什么正态分布在实践使用中非常的成功？

杰恩斯指出，正态分布在实践中成功的被广泛应用，主要是因为正态分布在数学方面的具有多种稳定性质，这些性质包括：

  * 两个正态分布密度的乘积还是正态分布
  * 两个正态分布密度的卷积还是正态分布，也就是两个独立正态分布的和还是正态分布
  * 正态分布$N(0, \sigma^2)$的傅立叶变换正规化为密度分布后还是正态分布
  * 中心极限定理保证了多个随机变量的求和效应将导致正态分布
  * 正态分布和其它具有相同均值、方差的概率分布相比，具有最大熵

前三个性质说明了正态分布一旦形成,就容易保持该形态的稳定， 兰登对于正态分布的推导也表明了，正态分布可以吞噬较小的干扰而继续保持形态稳定。后两个性质则说明，其它的概率分布在各种的操作之下容易越来越靠近正态分布。正态分布具有最大熵的性质，所以任何一个对指定概率分布的操作，如果该操作保持方差的大小，却减少已知的知识，则该操作不可避免的增加概率分布的信息熵，这将导致概率分布向正态分布靠近。

正由于正态分布多种的稳定性质，使得它像一个黑洞一样处于一个中心的位置，其它的概率分布形式在各种操作之下都逐渐向正态分布靠拢，杰恩斯把它描述为概率分布中重力现象(gravitating phenomenon)。

我们在实践中为何总是选择使用正态分布呢，正态分布在自然界中的频繁出现只是原因之一，杰恩斯认为还有一个重要的原因是正态分布的最大熵性质。在很多时候我们其实没有任何的知识知道数据的真实分布是什么， 但是一个分布的均值和方差往往是相对稳定的。因此我们能从数据中获取到的比较好的知识就是均值和方差，除此之外没有其它更加有用的信息量。因此按照最大熵的原理，我们应该在给定的知识的限制下，选择熵最大的概率分布，而这就恰好是正态分布。即便数据的真实分布不是正态分布，由于我们对真实分布一无所知，如果数据不能有效提供除了均值和方差之外的更多的知识，按照最大熵的原理，正态分布就是这时候最佳的选择。

当然正态分布还有更多令人着迷的数学性质，我们可以欣赏一下:

  * 二项分布 $B(n,p)$ 在 $n$很大逼近正态分布 $N(np, np(1-p))$
  * 泊松分布 $Poisson(\lambda)$ 在 $\lambda$ 较大时逼近正态分布 $N(\lambda,\lambda)$
  * $\chi^2_{(n)}$在 $n$很大的时候逼近正态分布 $N(n,2n)$
  * $t$分布在 $n$ 很大时逼近标准正态分布 $N(0,1)$
  * 正态分布的共轭分布还是正态分布
  * 几乎所有的极大似然估计在样本量$n$增大的时候都趋近于正态分布
  * 克拉美分解定理(之前介绍过)：如果 $X,Y$ 是独立的随机变量，且 $S=X+Y$ 是正态分布，那么 $X,Y$ 也是正态分布
  * 如果 $X,Y$ 独立且满足正态分布$N(\mu, \sigma^2)$, 那么 $X+Y$, $X-Y$ 独立且同分布，而正态分布是唯一满足这一性质的概率分布
  * 对于两个正态分布$X,Y$, 如果$X,Y$ 不相关则意味着$X,Y$独立，而正态分布是唯一满足这一性质的概率分布

**8. 大道至简,大美天成**

<p style="text-align: center">
  <em>To see a world in a grain of sand</em><br /> <em>And a heaven in a wild flower, </em><br /> <em>Hold infinity in the palm of your hand</em><br /> <em>And eternity in an hour.</em>
</p>

$$\overline{X} = \frac{X\_1 + X\_2 + \cdots + X_n}{n} $$
  
算术平均,极其简单而朴素的一个式子，被人们使用了千百年，在其身后隐藏着一个美丽的世界，而正态分布正是掌管这个美丽世界的女神。正态分布的发现与应用的最初历史，就是数学家们孜孜不倦的从概率论和统计学角度对算术平均不断深入研究的历史。中心极限定理在 1773年棣莫弗的偶然邂逅的时候，它只是一粒普通的沙子，两百多年来吸引了众多的数学家，这个浑金璞玉的定理不断的被概率学家们精雕细琢，逐渐的发展成为现代概率论的璀璨明珠。而在统计学的误差分析之中，高斯窥视了造物主对算术平均的厚爱，也发现了正态分布的美丽身影。殊途同归，那是偶然中的必然。一沙一世界，一花一天国, 算术平均或许只是一粒沙子，正态分布或许只是一朵花，它们却包含了一个广阔而美丽的世界，几百年来以无穷的魅力吸引着科学家和数学家们。
  
高尔顿他对正态分布非常的推崇与赞美,1886 年他在人类学研究所的就职演讲中说过一段著名的话：“我几乎不曾见过像误差呈正态分布这么美妙而激发人们无穷想象的宇宙秩序。如果古希腊人知道这条曲线，想必会给予人格化乃至神格化。它以一种宁静无形的方式在最野性的混乱中实施严厉的统治。暴民越多，无政府状态越显现，它就统治得越完美。他是无理性世界中的最高法律。当我们从混沌中抽取大量的样本，并按大小加以排列整理时，那么总是有一个始料不及的美妙规律潜伏在其中。”

概率学家卡克在他的自述传记《机遇之谜》(Enigmas of chance: An autobiography) 中描述他与正态分布的渊源：“我接触到正态分布之后马上被他深深的吸引，我感到难以相信，这个来自经验直方图和赌博游戏的规律，居然会成为我们日常生活数学的一部分。”另一位概率学家 Michel Loéve(1907-1979) 说：“如果我们要抽取列维的概率中心思想，那我们可以这样说，自从 1919 年以后，列维研究的主题曲就是正态分布，他一而再再而三的以她为出发点，并且坚决的又回到她&#8230;&#8230; 他是带着随机时钟沿着随机过程的样本路径作旅行的人。”美国国家标准局的顾问 W. J. Youden 用如下一段排列为正态曲线形状的文字给予正态分布极高的评价，意思是说：误差的正态分布规律在人类的经验中具有“鹤立鸡群”的地位，它在物理、社会科学、医学、农业、工程等诸多领域都充当了研究的指南，在实验和观测数据的解读中是不可或缺的工具。

&nbsp;

<p style="text-align: center">
  <strong><a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/youden-normal-curve/" rel="attachment wp-att-7070"><img class="aligncenter size-full wp-image-7070" alt="youden-normal-curve" src="https://cos.name/wp-content/uploads/2013/01/youden-normal-curve.jpg" width="819" height="304" srcset="https://cos.name/wp-content/uploads/2013/01/youden-normal-curve.jpg 819w, https://cos.name/wp-content/uploads/2013/01/youden-normal-curve-300x111.jpg 300w, https://cos.name/wp-content/uploads/2013/01/youden-normal-curve-500x185.jpg 500w" sizes="(max-width: 819px) 100vw, 819px" /></a>正态误差态分布律</strong>
</p>

几乎所有的人都或多或少的接触数学，虽然各自的目的不同，对数学的感觉也不同。工程师、科学家们使用数学是因为他简洁而实用，数学家们研究数学是因为它的美丽动人。像正态分布这样，既吸引着无数的工程师、科学家，在实践中被如此广泛的应用，又令众多的数学家为之魂牵梦绕的数学存在，在数学的世界里也并不多见。我在读研究生的时候，经常逛北大未名BBS 的数学板，有一个叫 ukim 的著名 ID 在精华区里面留下了一个介绍数学家八卦的系列《Heroes in My Heart》，写得非常的精彩，这些故事在喜欢数学的人群中也流传广泛。最后一个八卦是关于菲尔兹奖得主法国数学家托姆(René Thom)的，它曾经令无数人感动，我也借用来作为我对正态分布的八卦的结语：

_在一次采访当中，作为数学家的托姆同两位古人类学家讨论问题。谈到远古的人们为什么要保存火种时，一个人类学家说，因为保存火种可以取暖御寒；另外一个人类学家说，因为保存火种可以烧出鲜美的肉食。而托姆说，因为夜幕来临之际，火光摇曳妩媚，灿烂多姿，是最美最美的&#8230;&#8230;_

<p style="text-align: center">
  <a href="https://cos.name/2013/01/%e6%ad%a3%e6%80%81%e5%88%86%e5%b8%83%e7%9a%84%e5%89%8d%e4%b8%96%e4%bb%8a%e7%94%9f%e4%b8%8a/fire/" rel="attachment wp-att-7082"><img class="aligncenter  wp-image-7082" alt="fire" src="https://cos.name/wp-content/uploads/2013/01/fire.jpg" width="425" height="271" srcset="https://cos.name/wp-content/uploads/2013/01/fire.jpg 1025w, https://cos.name/wp-content/uploads/2013/01/fire-300x190.jpg 300w, https://cos.name/wp-content/uploads/2013/01/fire-472x300.jpg 472w" sizes="(max-width: 425px) 100vw, 425px" /></a>
</p>

**9. 推荐阅读**

_All knowledge is, in the final analysis, history. _
  
 _All sciences are, in the abstract, mathematics. _
  
 _All methods of acquiring knowledge are, essentially, through statistics._

_在终极的分析中，一切知识都是历史；_
  
 _在抽象的意义下，一切科学都是数学； _
  
 _在理性的基础上，所有的判断都是统计学。_

_&#8212; C. R. Rao_
  
_
  
_ 

本人并非统计学专业人士，只是凭个人兴趣做一点知识的传播。对统计学历史知识的介绍，专业性和系统性都不是我的目的，我更在乎的是趣味性，因为没有趣味就不会有传播。如果读完这段历史会让你觉得正态分布更加亲切，不再那么遥不可及，那我的目的达到了。如果正态分布是一滴水，我愿大家都能看到它折射出的七彩虹。

本文所使用的大多是二手资料，有些历史细节并没有经过严格的考证，对于历史资料一定程度上按照个人喜好做了取舍，本文主要基于如下的资料写成，对于历史细节感兴趣的，推荐阅读。

  * 陈希孺， 数理统计学简史，湖南教育出版社，2000
  * 蔡聰明，誤差論與最小平方法，数学传播 21(3):3-13，1994
  * 吴江霞，正态分布进入统计学的历史演化，2008
  * E.T. Jaynes, Probability Theory: The Logic of Science，Cambridge University Press，2003
  * Saul Stahl, The Evolution of the Normal Distribution, Mathematics Magazine, 1996
  * Kiseon Kim, Georgy Shevlyakov, Why Gaussianity, IEEE Signal Processing Magazine, 2008
  * Stephen M. Stigler, The History of Statistics: The Measurement of Uncertainty before, Belknap Press of Harvard University Press, 1990
  * L. Le Cam, The Central Limit Theorem Around 1935, Statistical Science 1(1):78-91, 1986
  * Hans Fischer, A History of the Central Limit Theorem: From Classical to Modern Probability Theory, Springer, 2010