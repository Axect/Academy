---
title: "Highschool Calculus"
author: [Tae Geun Kim]
date: 2018-07-25
subject: "Markdown"
keywords: [Markdown, Example]
subtitle: "For third-year Highschool Students"
titlepage: true
...


\newpage\null\thispagestyle{empty}\newpage

# Fundamental Theorem of Calculus

## Limit (극한)

*In a race, the quickest runner can never overtake the slowest,
since the pursuer must first reach the point whence the pursued
started, so that the slower must always hold a lead. \hspace{0.3cm} – Zeno*

\vspace{0.3cm}

그리스의 철학자 제논은 다음의 세 가지 역설을 주장하였다.

1) **아킬레우스와 거북** : 아킬레우스와 거북이가 경주를
한다고 하자. 거북이는 아킬레우스보다 $10m$앞에서 출발하며 아킬레우스는 거북이보다 10배 빠르다. 경주가 시작되고 아킬레우스가 $10m$에 도달하면 거북이는 $11m$에 있게 되고 아킬레우스가 $11m$에 도달하면 거북이는 $11.1m$에 있고, 아킬레우스가 $11.1m$에 도달하면 거북이는 $11.11m$에 있게 된다. 이 과정이 반복된다면 아킬레우스가 $t$번 동안 아무리 뛰어도 거북이는 항상 아킬레우스보다 $\left(\frac{1}{10} \right)^t m$앞
에 있으므로 아킬레우스는 거북이를 절대 따라잡을 수 없다.

2) **이분 역설** : A에서 B까지 가려면 A와 B 사이의 어떤 지점 C를 지나야 하고, 다시 A에서 C까지 가려고 하면 A와 C 사이의 한 지점 D를 지나야 하며, A에서 D까지 갈 때는 또 A와 D 사이에 있는 E를 지나야 한다. 이 과정을 반복하면 A와 B 사이가 아무리 짧아도 A에서 B까지 무한한 지점을 통과해야 하므로 물체는 움직일 수 없다.

3) **화살의 역설** : 화살을 과녁을 향해 쏘았다고 하자. 이때 어느 순간에 화살은 어느 한 점에 머무르고 있게 된다. 또한 그 다음 순간에도 화살은 어느 점에 머무른다.
이렇게 화살은 모든 순간에 머물러 있으므로 결국 움직일 수 없고 따라서 과녁에 도달할 수 없다.

\vspace{0.3cm}

$~$ \hspace{0.1cm} 이 세 가지 역설들은 단순히 그동안 당연히 여겨왔던 셀 수 있는 유한한 숫자들의 개념으로는 표현할 수 없다. 이외에도 다음과 같은 간단한 문제들도 있다.

\vspace{0.1cm}

1. $0.9999\cdots = 1$ 이 성립하는가?

2. $\displaystyle f(x) = \frac{\sin{x}}{x}$가 $x=0$ 근처로 갈 때, 어떤 값을 갖겠는가?

\vspace{0.1cm}

$~$ \hspace{0.1cm} 위 역설들과 문제들을 해결하려면 단순히 값을 대입하여 얻어내는 식으로는 문제를 풀 수 없다. 무한은 수가 아니며 따라서 무한이라는 수를 함수의 정의역으로 쓸 수 없다. 쉽게 말하자면 무한은 대입할 수 없다. 따라서 우리는 '근처'(Local)의 수학을 할 필요가 있다. 이를 하기위해 가장 먼저 필요한 것은 근처로 접근하는 것이다. 근처로 접근하기 위하여 우리는 먼저 '극한'이라는 도구를 알아야 한다.

\pagebreak

### Definition(정의)

극한의 정의는 다음과 같다.

\rule{\textwidth}{0.4pt}
**Limit**:  *어떤 임의의 양수 $\epsilon$에 대하여 $0<|x-a|<\delta$ 이면 $|f(x) - L| < \epsilon$ 을 만족하는 양수 $\delta$ 가 존재하면 $L$ 을 $f(x)$의 $a$에서의 극한값이라고 한다.*
\rule{\textwidth}{0.4pt}
