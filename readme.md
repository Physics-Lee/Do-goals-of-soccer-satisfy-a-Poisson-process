# What Will Happen on the Soccer Field in the Next Minute?

There is a famous saying in soccer: "The ball is round."

This means that anything is possible in soccer.

Hidden behind this phrase is a profound mathematical model.

------

In statistics, there is a sub-discipline called "stochastic processes."

In this field, there exists a type of process that satisfies a property: the future depends only on the present and is independent of the past.

Doesn't this sound very much like a soccer match?

This process is called a Markov process, and this property is known as Markovianity.

We know that scoring in soccer is an accumulative process, going from 0 to 1, then to 2, and so forth.

Statisticians refer to this accumulative process as a counting process. A counting process that has Markovian properties is called a Poisson process.

You might wonder whether goals in soccer truly exhibit Markovian properties, meaning whether the occurrence of a goal in the next minute really depends only on the current state and not on the past.

------

I have often heard that scoring in soccer follows a Poisson process.

To determine if it truly follows a Poisson process, one only needs to check if the intervals between goals follow an exponential distribution. It is easy to prove that the two are equivalent.

On the morning of July 14, 2023, I finally conducted a search on Google.

Many sources claim that scoring in soccer follows a Poisson process (or that the intervals between goals follow an exponential distribution), such as [this blog](https://allendowney.github.io/ThinkBayes2/chap08.html), but they do not support their claims with data.

On Google Scholar, I found [a data-supported paper](https://pubsonline.informs.org/doi/abs/10.1287/ited.3.2.64). The authors analyzed data from four World Cups between 1990 and 2002, finding that the distribution of intervals between goals was extremely similar to an exponential distribution. However, I think using data from only four World Cups is somewhat limited. What if I used data from all World Cups? Over a century, there have been just a few thousand goals at the World Cup, and FIFA should have preserved this precious data, right?

Subsequently, I searched on Google using `site:www.kaggle.com goal data of FIFA World Cup` and found [data on all goals from the 1930 to 2022 World Cups](https://www.kaggle.com/datasets/jahaidulislam/fifa-world-cup-all-goals-1930-2022-dataset) on Kaggle.

After analyzing the data, I found that the distribution of intervals between goals was extremely similar to an exponential distribution.

<img src = "/figures/histogram_connect two adjacent games.jpg" width=100% align="center">

------

Thus, at least on the soccer field, the future really does care only about the present, and not the past.

The leading team should not be complacent, and the trailing team should not give up.

If life were really like soccer, how wonderful that would be!