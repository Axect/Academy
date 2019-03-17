---
fontfamily: "libertine"
mainfont: "GFS Artemisa"
title: "Probability & Statistics"
author: [Tae Geun Kim]
date: 2019-03-17
subject: "Markdown"
keywords: [Markdown, Example]
subtitle: "For Highschool students"
titlepage: true
toc-own-page: true
...

\newpage\null\thispagestyle{empty}\newpage

# Permutation (순열)

## Definition

\begin{tcolorbox}[colback=white!5!white,colframe=black!30!blue, title=\textbf{Def 1.1 \hs Permutation (순열)}]
    서로 다른 $n$개 중 $r$개를 뽑아 일렬로 정렬하는 경우의 수를 \textbf{순열}이라 하며 정의는 다음과 같다.
    $$_nP_r = \frac{n!}{(n-r)!}$$
\end{tcolorbox}

모든 순열 문제는 줄 세우기 문제로 치환 가능하므로 줄 세우기 문제로 바꾼 후에 접근하는 것이 쉽다.

## Example

**1.** 집합 $A = \{1,2,3\}$에서 집합 $B = \{a,b,c,d,e,f\}$로의 함수 중에서 일대일 함수의 개수를 구하시오.

> 일대일 함수의 개수를 구하는 것은 $B$의 원소 중 $A$의 원소들에게 선택받을 3개를 골라 정렬하는 방법의 수와 같다.
따라서 답은 $_6P_3$ 이다.

\vspace{0.3cm}

**2.** 의자 6개가 나란히 설치되어 있다. 여학생 2명, 남학생 3명이 모두 의자에 앉을 때,
여학생이 이웃하지 않게 되는 경우의 수를 구하시오.

> 이런 경우는 이웃한 경우를 빼는 것이 쉽다. 여학생 2명이 이웃하는 경우에는, 여학생 2명을 하나의 묶음으로 보고 정렬하게 된다. 
또한, 정렬하고 난 후 여학생들끼리의 정렬도 고려해야하므로 계산식은 다음과 같다.
$$6! - 5! \times 2!$$

