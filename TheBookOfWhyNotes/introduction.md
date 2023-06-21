# INTRODUCTION: MIND OVER DATA

- 下面这段话我觉得写得非常好
  This book tells the story of a science that has changed the way we distinguish facts from fiction and yet has remained under the radar of the general public. The consequences of the new science are already impacting crucial facets of our lives and have the potential to affect more, from the development of new drugs to the control of economic policies, from education and robotics to gun control and global warming. Remarkably, despite the diversity and apparent incommensurability of these problem areas,
  the new science embraces them all under a unified framework that was practically nonexistent two decades ago.
  The new science does not have a fancy name: I call it simply “causal inference,” as do many of my colleagues. Nor is it particularly high-tech. The ideal technology that causal inference strives to emulate resides within our own minds. Some tens of thousands of years ago, humans began to realize that certain things cause other things and that tinkering with the former can change the latter. No other species grasps this, certainly not to the extent that we do. From this discovery came organized societies, then towns and cities, and eventually the science- and technology-based civilization we enjoy today. **[All because we asked a simple question: Why?]()**

> By the way, 这本书的文笔真的很好！

- 作者提出了这门学科诞生之前遇到的困难：

  - The most serious impediment, in my opinion, has been the fundamental gap between the vocabulary in which we
    cast causal questions and the traditional vocabulary in which we communicate scientific theories.
    > 想起作者在 preface 里面写到这门学科被数学化了，和这里呼应了~
  - 然后以下面这个显式的因果关系过渡
    To appreciate the depth of this gap, imagine the difficulties that a scientist would face in trying to express some obvious causal relationships—say, that the barometer reading B tracks the atmospheric pressure P. We can easily write down this relationship in an equation such as B = kP, where k is some constant of proportionality. The rules of algebra now permit us to rewrite this same equation in a wild variety of forms, for example, P = B/k, k = B/P, or B–kP = 0. They all mean the same thing—that if we know any two of the three quantities, the third is determined. None of the letters k, B, or P is in any mathematical way privileged over any of the others. How then can we express our strong conviction that it is the pressure that causes the barometer to change and not the other way around? **And if we cannot express even this, how can we hope to express the many other causal convictions that do not have mathematical formulas, such as that the rooster’s crow does not cause the sun to rise?**

- 作者继续娓娓道来，引出发展历史

  - scientific tools are developed to meet scientific needs.
  - As as scientific curiosity increased and we began posing causal questions in complex legal, business, medical, and policy-making situations, we found ourselves lacking the tools and principles that mature science should provide.

  作者说这是一种 belated awakening, 然后讲述了统计学的出现，也是一种 belated awakening

  - 而统计学，一种 causality-free enterprise 恰是在对因果需求浮现的时候 兴起的
    - the need for a theory of causation began to surface at the same time that statistics came into being.
  - In fact, modern statistics hatched from the causal questions that Galton and Pearson asked about heredity and their ingenious attempts to answer them using cross-generational data. Unfortunately, they failed in this endeavor, and rather than pause to ask why, they declared those questions off limits and turned to developing a thriving, causality-free enterprise called statistics.
    > 事实上，现代统计学是从高尔顿和皮尔森提出的关于遗传的因果问题，以及他们使用跨代数据来回答这些问题的巧妙尝试中孵化出来的。不幸的是，他们在这方面的努力失败了，他们没有停下来问为什么，而是宣布禁止这些问题，转而发展一项蓬勃发展的、没有因果关系的事业，即统计学。

- 在科学发展的一个关键时期,因果推理本来有机会获得自己的语言来表达,但这个机会被错过了。在随后的几十年中,因果推理被宣布为非科学的,被迫“地下化”

  - This was a critical moment in the history of science. The opportunity to equip causal questions with a language of their own came very close to being realized but was squandered. In the following years, these questions were
    declared unscientific and went underground.

- 除了遗传学家西瓦尔·怀特的努力外,因果推理的语言基本上被禁止使用了半个世纪。

  > 下面这句话写的真好！

  And when you prohibit speech, you prohibit thought and stifle principles, methods, and tools. **当你禁止言论时，你就禁止了思想，扼杀了原则、方法和工具。**

- 由于这种禁令,管理因果推理的数学工具被认为是不必要的。统计学仅专注于如何总结数据,而不是如何解释数据。西瓦尔·怀特在 1920 年代发明的路径分析是个令人瞩目的例外,但它在统计学和相关学科中长期得不到应有的重视和发展。

  - Because of this prohibition, mathematical tools to manage causal questions were deemed unnecessary, and statistics focused exclusively on how to summarize data, not on how to interpret it.

- 直到 1980 年代,因果推理才开始有所发展。在此之前,统计学及其影响下的许多学科仍处于“禁令”时期,错误地认为所有的科学问题的答案都在数据中,只需要巧妙的数据挖掘技巧就可以揭示。

  - What should have been the first step toward causal inference remained the only step until the 1980s. The
    rest of statistics, including the many disciplines that looked to it for guidance,remained in the Prohibition era, falsely believing that the answers to all scientific questions reside in the data, to be unveiled through clever data mining tricks

- 今天,我们生活在一个认为大数据可以解决所有问题的时代。但作者希望通过这本书来说服读者,数据本质上是愚蠢的。数据可以告诉你服用某种药物的人康复得更快,但数据无法告诉你为什么。也许服药的人之所以康复得更快,是因为他们有能力付得起药费,即使不吃那种药也会康复得一样快

  - Much of this data-centric history still haunts us today. We live in an era that presumes Big Data to be the solution to all our problems. Courses in“data science” are proliferating in our universities, and jobs for “data scientists” are lucrative in the companies that participate in the “data economy.” But I hope with this book to convince you that data are profoundly dumb. Data can tell you that the people who took a medicine recovered faster than those who did not take it, but they can’t tell you why. Maybe those who took the medicine did so because they could afford it and would have recovered just as fast without it.

- 4
- 5
- 6
- 7
- 8
- 9
- 10
