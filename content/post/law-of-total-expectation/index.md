---
title: Law of Total Expectation
subtitle: 

# Summary for listings and search engines
summary: 

# Link this post with a project
projects: []

# Date published
date: "2020-03-16T00:00:00Z"

# Date updated
lastmod: "2020-03-16T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- Math

categories:
- Math
---

## Law of Total Expectation

PRML의 74pg. Bayesian statistics에 대한 설명 중 다음과 같은 수식이 나온다.
$$
\mathbb{E}_\theta[\theta] = \mathbb{E}_\mathcal{D}[\mathbb{E}_\theta[\theta|\mathcal{D}]]
$$
이 식의 직관적인 의미가 와 닿지 않았어서, 이 포스트를 통해 정리한다.



### Intuition

이 식에 대한 Bishop의 해석은 다음과 같다.

> Posterior mean of $\theta$, averaged over the distribution generating the data, is equal to the prior mean of $\theta$.

우리가 estimate하고자하는 parameter가 있고, 그 parameter에 대한 prior distribution이 있다고 가정하자. 또한, Bayesian inference를 수행하기 위해 새롭게 observe한 dataset이 있고, 우리는 Bayesian statistic을 이용해 parameter의 posterior를 구할 수 있다. 이 때, 우리가 observe한 dataset이 어떠한 underlying distribution $p(\mathcal{D})$를 가진다고 생각하면, dataset이 사실은 여러 realization이 가능하다고 생각할 수 있다. "Averaged over the distribution generating the data"는 이를 뜻한다. **따라서 어떤 data의 여러 realization이 있을 때, 그 각각의 realization에서의 posterior mean이 존재하고, 그 각각의 posterior mean의 average value는 결국 prior mean과 같아진다는 뜻이다.**



continuous variable을 써서는 직관적이지 않으니, discrete random variable로 해석을 해보자. $A_1, A_2, A_3$라는 event가 있고, 그와는 independent하게 $B$라는 event가 있으면, law of total probability를 통해 다음과 같은 식을 쓸 수 있다.


$$
p(B) = p(A_1)p(B|A_1) + \dots + p(A_n)p(B|A_n)
$$

이 때,

$$
B = [X = x]
$$

라고 주어지면, 위 식을 pmf로 볼 수 있으며, 이에 따라

$$
p_X(x) = p(A_1)p_{X|A_1}(x) + \dots + p(A_n)p_{X|A_n}(x)
$$

임을 알 수 있다. 이는 모든 $x$에 대해 valid하기 때문에, 양 변에 $x$를 곱하고 이에 대한 sum을 취하면

$$
\sum_{x}xp_x(x) = p(A_1)\sum_{x}xp_{x|A_1}(x) + \dots + p(A_n)\sum_{x}xp_{x|A_n}(x)
$$

을 얻는다. 각 sum은 expectation의 정의에 따라 expectation, 또는 conditional expectation으로 바꿔 쓸 수 있다. 따라서,

$$
\mathbb{E}[x] = p(A_1)\mathbb{E}[x|A_1] + \dots + p(A_n)\mathbb{E}[x|A_n]
$$

이는 맨 위의 law of total expectation의 discrete version이며, 해석을 해보자면 다음과 같다.

$A_k$라는 event set이 있을 때, 각 event set에서의 expectation의 event set에 대한 expectation이 전체 expectation과 동일하다.

이를 continuous random variable에서 보자면, PRML에 나와 있는 식과 같이

$$
\mathbb{E}_\theta[\theta] =\int p(\theta)\theta\,d\theta \\
\mathbb{E}_\mathcal{D}[\mathbb{E}_\theta[\theta|\mathcal{D}]] = \int\{\int\theta p(\theta|\mathcal{D})\,d\theta\}p(\mathcal{D})\,d\mathcal{D}
$$

임을 확인할 수 있다.

**Total Expectation Theroem **은 **Law of iterated expectations**라는 말로도 표현된다. 후자가 더 general한 concept로 볼 수 있다.

$$
\mathbb{E}[\mathbb{E}[X|Y]] = \mathbb{E}[g(Y)]
$$

where

$$
g(Y) = \mathbb{E}[X|Y = y]
$$

여기서 $g(Y)$는 conditional expectation이고, 따라서 다시 풀어쓰면

$$
\mathbb{E}[g(Y)] \\
= \sum_yg(y)p_Y(y) \\
= \sum_y\mathbb{E}[X|Y=y]p_Y(y) \\
= \mathbb{E}[X]
$$

임을 다시 한 번 확인할 수 있다. 이 property는 이후에 **Law of total variance**를 증명하는 데에 쓰인다.

## Law of Total Variance

$$
var(X) = \mathbb{E}[var(X|Y)] + var(\mathbb{E}[X|Y])
$$

식만 봤을 때는 이 식이 무엇을 뜻하는지도 모호하다. 일단 이를 증명하고 가자면,

$$
var(X|Y) = \mathbb{E}[X^2|Y] - (\mathbb{E}[X|Y])^2
$$

임을 이용하면 되는데,

$$
\mathbb{E}[var(X|Y)] = \mathbb{E}[\mathbb{E}[X^2|Y]] - \mathbb{E}[(\mathbb{E}[X|Y])^2] \\
= \mathbb{E}[X^2] - \mathbb{E}[(\mathbb{E}[X|Y])^2]
$$

임을 확인 할 수 있다. 두번째 inequality는 law of iterated expectation을 이용한 것이다.

$$
var(\mathbb{E}[X|Y]) = \mathbb{E}(\mathbb{E}[X|Y]^2) - (\mathbb{E}(\mathbb{E}[X|Y]))^2 \\
= \mathbb{E}(\mathbb{E}[X|Y]^2) - \mathbb{E}[X]^2
$$

이를 derive할 때 다시 한번 law of iterated expectation를 이용했다.

위와 아래식을 더하면 기존 variance를 얻을 수 있다.

### Intuition

Law of total variance를 Bayesian viewpoint에서 보자면, conditioning을 dataset에 대해서 했다고 생각할 수 있다. PRML의 notation을 가져오자면

$$
var_\theta[\theta] = \mathbb{E}_\mathcal{D}[var_\theta[\theta|\mathcal{D}]] + var_\mathcal{D}[\mathbb{E}_\theta[\theta|\mathcal{D}]]
$$

인데, 여기서 좌변은 어떠한 observation도 없었을 때의 prior variance로 생각할 수 있다. 반면, 우변의 첫번째 term은 **posterior variance의 average value**이고, 두번째 term은 **posterior mean의 variance**이다. 여기서 두 번째 term은 positive value이기에, 평균적으로 보자면 **posterior variance가 prior variance보다 작아진다.** 다시말해, **어떤 dataset에 대한 conditioning이 있을 때 variance는 줄게된다.**
