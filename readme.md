# 下一分钟，足球场上将发生什么？

足球里有一句名言：足球是圆的。

这句话在揭示一个深刻的事实：在足球比赛中，什么都有可能发生。

可是，我们是否能从科学的角度来解释这句话呢？

让我们引入一种被称为“随机过程”的概念。在这个领域里，有一种特别的过程叫做马尔可夫过程。马尔可夫过程有一个特性：未来只与现在有关，而与过去无关。听起来是不是很像足球比赛？

我们知道，足球比赛中的进球是一个累加过程，从0到1，再到2，以此类推。这种累加过程在统计学中被称为计数过程。而有马尔可夫性质的计数过程被称为泊松过程。

你可能会问，足球比赛中的进球究竟是否满足马尔可夫过程的特性，也就是说，下一分钟有没有进球真的只取决于现在的状态，而和过去无关吗？

我一直听说，足球比赛的进球实际上就是符合泊松过程的。为了验证这个观点，我于2023年7月14日在谷歌上进行了一番搜索。许多地方都声称足球比赛的进球符合泊松过程（或者声称进球间的时间间隔符合指数分布），如[这篇博客](https://allendowney.github.io/ThinkBayes2/chap08.html)，但他们没有数据来支持他们的观点。

然后，在谷歌学术上，我找到了[一篇有数据支持的论文](https://pubsonline.informs.org/doi/abs/10.1287/ited.3.2.64)。作者统计了1990-2002四届世界杯的数据，发现进球间的时间间隔的分布与指数分布极其相似。但我觉得，只用四届世界杯的数据也太少了点。如果我用所有的世界杯的数据呢？一百年来，世界杯一共也就几千个进球，FIFA应该会保存这些珍贵的数据吧？

随后，我在Google上使用`site:www.kaggle.com goal data of FIFA World Cup`搜索，找到了[1930-2022世界杯的全部进球数据](https://www.kaggle.com/datasets/jahaidulislam/fifa-world-cup-all-goals-1930-2022-dataset)。我同样发现，进球间的时间间隔的分布和指数分布极其相似。

<img src = "/figures/histogram_connect two adjacent games.jpg" width=100% align="center">

---

所以，足球场上，未来的进球真的只在乎现在，一切皆有可能。

无论你是胜利在望的一方，还是暂时落后的一方，都不应过早庆祝或失望，因为在足球场上，每分钟都充满着未知和惊喜。

因此，足球，就是那个永恒变动的圆。

