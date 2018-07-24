---
title: "Function"
author: [Tae Geun Kim]
date: 2018-07-24
subject: "Markdown"
keywords: [Markdown, Example]
subtitle: "For First-year Highschool Students"
titlepage: true
...

# Basic Concepts of Function (함수의 기본 개념들)

## Notation (표기법)

* 집합기호
    * $\mathbb{N}$ : 자연수집합
    * $\mathbb{Z}$ : 정수집합
    * $\mathbb{Q}$ : 유리수집합
    * $\mathbb{R}$ : 실수집합
* 논리기호
    * $\forall$ : 모든 ~ 에 대하여
    * $\exists$ : 존재한다.

## Definition (정의)

함수란 두 집합간의 대응관계를 나타낸 것으로 $f: X \rightarrow Y$ 라 할 때, 다음 두 조건을 만족한다.

1. $X$의 모든 원소 $x$에 대하여 $f(x)$가 존재한다.
2. $X$의 원소 $x$에 대하여 단 하나의 $f(x)$만이 존재한다.

이 때, 집합 $X$를 함수 $f$의 **정의역**(domain)이라고 부르며 $Y$를 함수 $f$의 **공역**(range)이라 한다.
또한, $f(X)$를 **치역**(image)이라고 부르는데 치역의 정의는 다음과 같다.
$$f(X) = \left\{f(x) | x \in X \right\} $$

### Examples
1. 함수 $f:\{1,2,3\} \rightarrow \mathbb{Z}$ 가 $f(x) = x^2 -4$로 정의되었을 때, 함수 $f$의 치역은 $\{-3, 0, 5\}$이다. 
2. 함수 $f:\mathbb{R} \rightarrow \mathbb{R}$이 $f(x) = x^2$으로 정의되었을 때, 함수 $f$의 치역 $f(\mathbb{R})$은 $\{y | y\in\mathbb{R}, y\geq 0\}$이다.
3. 가우스 함수 $f(x) = [x]$의 치역은 $\mathbb{Z}$이다.

## Important Functions (중요 함수들)

1. 함수 $f: X \rightarrow Y$에 대해 $x_1 \neq x_2$ 이면 $f(x_1)\neq f(x_2)$을 만족하는 함수를 일대일 함수라고 한다. 또는 $f(x_1) = f(x_2)$ 이면 $x_1 = x_2$를 만족하는 함수라고 정의하기도 한다. (참을 증명할 때는 후자, 반례를 보일 때는 전자를 사용하면 된다.)
2. 함수 $f: X\rightarrow Y$가 일대일 함수이고 $f(X) = Y$이면 함수 $f$를 일대일 대응이라고 한다.
3. 함수 $f : X \rightarrow X$가 $f(x) = x$를 만족하면 그 함수를 항등함수라고 한다.
4. 함수 $f: X \rightarrow Y$가 $f(x) = c$를 만족하는 함수를 상수함수라고 부른다.

\pagebreak

### Examples

Q1. 함수 $f(x) = x^3$이 일대일 대응임을 보여라.

A1. $f(x_1) = f(x_2)$라 가정하자. 그렇다면 $x_1^3 = x_2^3$이 되는데 좌변으로 이항한 후 인수분해 공식을 사용하면 $(x_1 - x_2)(x_1^2 + x_1 x_2 + x_2^2) = 0$이 된다. 이때, 뒤의 식은 판별식이 0보다 작기 때문에 근을 가지지 못한다. 따라서 $x_1 = x_2$이다. 또한, $f$의 치역과 공역이 모두 실수 전체로 같으므로 함수 $f$는 일대일 대응이다.

\vspace{0.5cm}

Q2. 함수 $f(x) = x^2$이 일대일 함수가 아님을 보여라.

A2. $x_1 = 1,\, x_2 = -1$에 대해 $x_1 \neq x_2$이지만, $f(x_1) = 1 = f(x_2)$이므로 함수 $f$는 일대일 함수가 아니다.

### Problems

1. $X = \{0,1,2,3,4\}$와 $f: X \rightarrow X$에 대한 다음 명제들의 참, 거짓을 판별하시오.

    1) $f(x) = x+1$은 함수이다.

    2) $f(x) = 4 - x$는 일대일 대응인 함수이다.

    3) $f(x) = 0 \cdot x$는 함수이다.

    4) $f(x) = |3 - x|$는 일대일 대응이다.

    5) 일대일 대응인 함수 $f$는 100개 이상이다.

\vspace{0.5cm}

2. 항등함수가 일대일 대응임을 증명하여라.

\vspace{3cm}

3. $f(x) = [x]$가 일대일 대응이 되게 만드려면 정의역과 공역을 어떻게 구성해야 할 지 서술하시오.

\pagebreak

# Composit Function (합성함수)

## Definition

집합 $X,Y,Z$에 대해, 함수 $f: X \rightarrow Y$, $g: Y \rightarrow Z$가 존재한다고 할 때, 함수 $g \circ f : X \rightarrow  Z$를 $f$와 $g$의 합성함수라고 부르고 다음과 같이 정의한다.
\begin{equation*}
    (g \circ f)(x) = g(f(x)), ~~ \forall x \in X
\end{equation*}

### Examples

1. 함수 $f(x) = x^2$, $g(x) = 2x+1$에 대하여 $(f\circ g)(x) = (2x + 1)^2$ 이고 $(g \circ f)(x) = 2x^2 + 1$ 이다.

2. 함수 $f(x) = -2x + 1$이고, 함수 $g$가 다음과 같이 정의되었다고 한다.
\begin{equation*}
    g(x)=
    \begin{cases}
        x + 1 & (x < 1) \\
        x^2 - 1 & (x \geq 1)
    \end{cases}
\end{equation*}
이때, $(f \circ g)(x)$ 와 $(g \circ f)(x)$는 다음과 같이 구할 수 있다.
\begin{equation}
    (f \circ g)(x) =
    \begin{cases}
        -2(x + 1) + 1 & (x < 1) \\
        -2(x^2 - 1) + 1 & (x \geq 1)
    \end{cases}
\end{equation}
\begin{equation}
    (g \circ f)(x) =
    \begin{cases}
        -2x + 1 + 1 & (f(x) < 1) \\
        (-2x + 1)^2 - 1 & (f(x) \geq 1)
    \end{cases}
\end{equation}
이를 정리하면 답은 다음과 같다.
\begin{equation}
    (f \circ g)(x) =
    \begin{cases}
        -2x - 1 & (x < 1) \\
        -2x^2 + 3 & (x \geq 1)
    \end{cases}
\end{equation}
\begin{equation}
    (g \circ f)(x) =
    \begin{cases}
        -2x + 2 & (x > 0) \\
        4x^2 - 4x & (x \leq 0)
    \end{cases}
\end{equation}

\pagebreak

### Problems

1. 함수 $f: X \rightarrow Y$와 $g: Y \rightarrow Z$가 모두 일대일 함수일 때, \hspace{0.1cm} $g \circ f$도 일대일 함수 임을 증명하시오.

\vspace{5cm}

2. 함수 $f: \mathbb{R} \rightarrow \mathbb{R}$와 $g: \mathbb{R} \rightarrow \mathbb{R}$가 각각 $f(x) = x^2 + 2$, \hspace{0.1cm} $g(x) = 2x - 1$로 정의되었을 때, 함수 $f \circ g$와 $g \circ f$를 구하여라.

\vspace{3cm}

3. [인하대학교 2015 논술] 함수 $f: \mathbb{R} \rightarrow \mathbb{R}$가 다음과 같을 때, 함수 $(f \circ f)(x)$의 그래프를 그리시오.
\begin{equation*}
    f(x) = 
    \begin{cases}
        -x-1 & (x < 0) \\
        2x-1 & (x \geq 0)
    \end{cases}
\end{equation*}