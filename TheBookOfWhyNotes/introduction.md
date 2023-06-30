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

- 但其实数据本身并不足够

  Over and over again, in science and in business, we see situations where mere data aren’t enough. Most big-data enthusiasts, while somewhat aware of these limitations, continue the chase after data-centric intelligence, as if we were still in the Prohibition era.

- 因果模型的出现：作者提到，现代科学家通过精心构建的因果模型可以解决过去被认为是无法解决甚至是超出科学探究范畴的问题。例如，仅仅一百年前，香烟是否对健康造成危害这个问题会被认为是不科学的。在任何有声望的统计期刊中，提到“因果”或“效应”这两个词都会引起一场争议的风暴。甚至在二十年前，向统计学家提出类似“是阿司匹林止痛了吗？”这样的问题就像是问他是否相信巫术。但是现在，流行病学家、社会科学家、计算机科学家和至少一些开明的经济学家和统计学家经常提出这样的问题，并用数学的准确性回答它们。

   Nowadays, thanks to carefully crafted causal models, contemporary scientists can address problems that would have once been considered unsolvable or even beyond the pale of scientific inquiry. For example, only a hundred years ago, the question of whether cigarette smoking causes a health hazard would have been considered unscientific. The mere mention of the words “cause” or “effect” would create a storm of objections in any reputable statistical journal. Even two decades ago, asking a statistician a question like “Was it the aspirin that stopped my headache?” would have been like asking if he believed in voodoo. To quote an esteemed colleague of mine, it would be “more of a cocktail conversation topic than a scientific inquiry.” But today, epidemiologists, social scientists, computer scientists, and at least some enlightened economists and statisticians pose such questions routinely and answer them with mathematical precision.

- 作者将上面这种变化称为“因果革命”，并指出它背后的数学秘密可以被描述为"因果计算"，它回答了关于因果关系的一些最困难的问题

   To me, this change is nothing short of a revolution. I dare to call it the Causal Revolution, a scientific shakeup that embraces rather than denies our innate cognitive gift of understanding cause and effect. The Causal Revolution did not happen in a vacuum; it has a mathematical secret behind it which can be best described as a calculus of causation, which answers some of the hardest problems ever asked about cause-effect relationships

- "因果计算"的两种语言：

  | 形式                          | 描述                                                         |
  | ----------------------------- | ------------------------------------------------------------ |
  | 因果图（Causal Diagrams）     | 使用点和箭头的图片形式来总结我们已知的科学知识。点代表感兴趣的量，也称为“变量”，箭头表示这些变量之间已知或疑似的因果关系，即哪个变量“听取”哪些其他变量的影响。这些图形易于绘制、理解和使用。 |
  | 符号语言（Symbolic Language） | 类似代数的符号语言，用于表达我们想要了解的内容。符号语言可以用数学表达式或假设清单的形式表示，描述因果关系结构。无论使用哪种形式，模型都应以某种程度上的定性方式反映数据生成过程，即环境中的因果力量如何塑造生成的数据。 |

- 因果革命的一个重要成就是解释了如何在没有实施干预的情况下预测其效果。这一成就的实现离不开两个关键因素：

  - 首先，我们定义了do运算符，使我们能够提出正确的问题；
  - 其次，我们设计了一种非侵入性的模拟方法来模拟do运算符的效果。这些创新使得我们能够在不进行实际干预的情况下预测干预的效果。

  One of the crowning achievements of the Causal Revolution has been to explain how to predict the effects of an intervention without actually enacting it. It would never have been possible if we had not, first of all, defined the do-operator so that we can ask the right question and, second, devised a way to emulate it by noninvasive means

- counterfactual 反事实

  - Counterfactuals（反事实）是因果推理中的一种表达方式，用于描述与实际情况相反的假设情况。
  - 反事实思考在因果推断中起着重要作用，通过比较实际观测结果与反事实情况下的预测结果，可以评估因果关系。

  - 传统统计学只能总结数据，无法提供问这类问题的语言，而因果推断提供了一种表达方法和解决方案。

  - 在许多情况下，可以通过算法来模拟人类的回顾性思维，根据观测世界的信息提供关于反事实世界的答案。

  - 反事实推理虽然无法经验观察证实或否定答案，但我们的思维对于可能性和可能性的判断非常可靠和可重复。

  - 反事实是道德行为和科学思考的基石，反思过去行为并设想替代情景是自由意志和社会责任的基础。

  - 反事实的算法化使得思考机器能够参与到这种唯一的人类思考世界的方式中。

- 然后作者从人工智能的视角研究因果推理,提出了以下几点思考:

  - 让机器学会一个主题,关键在于能将其教给机器人。这需要使用清晰的语言和符号,并强调表达和推理能力。
  - 语言决定思维。如果没有理解问题的语言,就无法提问和求解。
  - 因果推理的语言和符号体系发展成熟,激发了作者学习它的兴趣。
  - 作者认为因果关系理解能提高机器智能。机器缺乏因果理解是当前限制其智能的主要障碍。
  - 作者认为强人工智能是可实现的,正是因为因果性是其一部分。

  具体来说,具备因果推理模块可以:

  - 使机器能够反思自身错误和软件短板
  - 让机器成为有道德意识的实体
  - 让机器可以自然地与人类讨论其自身选择和意图

  总的来说，作者从人工智能的角度检视因果推理,认为因果理解可以提高机器的智能水平,然而关键还在于能够清晰地表达和交流因果概念



---

- 接着作者介绍了各章的梗概

---

- 最后下面这段结尾的话我觉得写得也很好

  If I could sum up the message of this book in one pithy phrase, it would be that you are smarter than your data. Data do not understand causes and effects; humans do. I hope that the new science of causal inference will enable us to better understand how we do it, because there is no better way to understand ourselves than by emulating ourselves. In the age of computers, this new understanding also brings with it the prospect of amplifying our innate abilities so that we can make better sense of data, be it big or small.