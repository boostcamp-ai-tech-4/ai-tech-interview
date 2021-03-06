## ๐ Table of Contents

- [๋ฒ ๋ฅด๋์ด ๋ถํฌ](#1)
- [์ดํญ ๋ถํฌ](#2)
- [์นดํ๊ณ ๋ฆฌ ๋ถํฌ](#3)
- [๋คํญ ๋ถํฌ](#4)
- [๊ฐ์ฐ์์ ์ ๊ท ๋ถํฌ](#5)
- [t ๋ถํฌ](#6)
- [์นด์ด์ ๊ณฑ ๋ถํฌ](#7)
- [F ๋ถํฌ](#8)
- [๋ฒ ํ ๋ถํฌ](#9)
- [๊ฐ๋ง ๋ถํฌ](#10)

---

## #1

#### ๋ฒ ๋ฅด๋์ด ๋ถํฌ

์ฐ์  ๋ฒ ๋ฅด๋์ด ์ํ์ด๋ ๊ฒฐ๊ณผ๊ฐ ๋ ๊ฐ์ง ์ค ํ๋๋ง ๋์ค๋ ๊ฒ์ ๋งํ๋ค. ๋ฒ ๋ฅด๋์ด ํ๋ฅ ๋ณ์๋ ์ํ๊ฒฐ๊ณผ๊ฐ 0 ๋๋ 1์ด ๋์ค๋ฏ๋ก ์ด์ฐํ๋ฅ ๋ณ์์ด๋ค.

- `pmf` : <!-- $Bern(x;\theta) = \theta^x(1-\theta)^{1-x}$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=Bern(x%3B%5Ctheta)%20%3D%20%5Ctheta%5Ex(1-%5Ctheta)%5E%7B1-x%7D">
- `expectation` : <!-- $E[X] = \theta$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=E%5BX%5D%20%3D%20%5Ctheta">
- `variance` : <!-- $Var[X] = \theta ( 1-\theta)$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=Var%5BX%5D%20%3D%20%5Ctheta%20(%201-%5Ctheta)">

#### References

- [ํ๋ฅ ๋ถํฌ : ๋ฒ ๋ฅด๋์ด๋ถํฌ, ์ดํญ๋ถํฌ, ์นดํ๊ณ ๋ฆฌ๋ถํฌ, ๋คํญ๋ถํฌ - Fall in Machine-Learning](https://imjuno.tistory.com/entry/basicdistribution)
- [8.2 ๋ฒ ๋ฅด๋์ด๋ถํฌ์ ์ดํญ๋ถํฌ - ๋ฐ์ดํฐ ์ฌ์ด์ธ์ค ์ค์ฟจ](https://datascienceschool.net/02%20mathematics/08.02%20%EB%B2%A0%EB%A5%B4%EB%88%84%EC%9D%B4%EB%B6%84%ED%8F%AC%EC%99%80%20%EC%9D%B4%ED%95%AD%EB%B6%84%ED%8F%AC.html)

---

## #2

#### ์ดํญ ๋ถํฌ

๋ฒ ๋ฅด๋์ด ์ํ์ N๋ฒ ์ํํ ๊ฒ์ ๋งํ๋ค. ์๋ฅผ ๋ค์ด, ๋์  ๋์ง๊ธฐ๋ฅผ 10๋ฒ ๋์ ธ์ ์๋ฉด์ด ๋์จ ํ์๋ฅผ ํ๋ฅ  ๋ณ์๋ก ๋๋ค. ๋ง์ฐฌ๊ฐ์ง๋ก ์ํ ๊ฒฐ๊ณผ๊ฐ ํ์๋ก ๋์ค๋ฏ๋ก ์ด์ฐํ๋ฅ ๋ณ์์ด๋ค.

- `pmf` : <!-- $Bin(x;N, \theta) = \left(\begin{array}{c}N\\ x\end{array}\right) \theta^N (1-\theta)^{N-x}$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=Bin(x%3BN%2C%20%5Ctheta)%20%3D%20%5Cleft(%5Cbegin%7Barray%7D%7Bc%7DN%5C%5C%20x%5Cend%7Barray%7D%5Cright)%20%5Ctheta%5EN%20(1-%5Ctheta)%5E%7BN-x%7D">
- `expectation` : <!-- $E[X] = N\theta$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=E%5BX%5D%20%3D%20N%5Ctheta">
- `variance` : <!-- $Var[X] = N\theta ( 1-\theta)$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=Var%5BX%5D%20%3D%20N%5Ctheta%20(%201-%5Ctheta)">

#### References

- [ํ๋ฅ ๋ถํฌ : ๋ฒ ๋ฅด๋์ด๋ถํฌ, ์ดํญ๋ถํฌ, ์นดํ๊ณ ๋ฆฌ๋ถํฌ, ๋คํญ๋ถํฌ - Fall in Machine-Learning](https://imjuno.tistory.com/entry/basicdistribution)
- [8.2 ๋ฒ ๋ฅด๋์ด๋ถํฌ์ ์ดํญ๋ถํฌ - ๋ฐ์ดํฐ ์ฌ์ด์ธ์ค ์ค์ฟจ](https://datascienceschool.net/02%20mathematics/08.02%20%EB%B2%A0%EB%A5%B4%EB%88%84%EC%9D%B4%EB%B6%84%ED%8F%AC%EC%99%80%20%EC%9D%B4%ED%95%AD%EB%B6%84%ED%8F%AC.html)

---

## #3

#### ์นดํ๊ณ ๋ฆฌ ๋ถํฌ

์นดํ๊ณ ๋ฆฌ ๋ถํฌ(Categorical distribution)๋ ๋ฒ ๋ฅด๋์ด ๋ถํฌ๋ฅผ ํ์ฅํ ๊ฐ๋์ด๋ค. ์ฆ ์นดํ๊ณ ๋ฆฌ ์ํ(์ฌ๋ฌ๊ฐ์ ์นดํ๊ณ ๋ฆฌ ์ค ํ๋๋ฅผ ์ ํํ๋ ์คํ)์ ๊ฒฐ๊ณผ๋ ์นดํ๊ณ ๋ฆฌ ๋ถํฌ๋ฅผ ๋ฐ๋ฅด๊ฒ ๋๋ค. ์นดํ๊ณ ๋ฆฌ ๋ถํฌ๋ฅผ ๋์ ํ๋ฉด ๋คํญ๋ถํฌ๋ฅผ ์ป๊ฒ ๋๋ค.

์นดํ๊ณ ๋ฆฌ ํ๋ฅ ๋ณ์๋ one-hot vector๋ก ํํํ  ์ ์๋ค. ์๋ฅผ ๋ค์ด, ์ฃผ์ฌ์์ ๊ฒฝ์ฐ K=6์ธ ์นดํ๊ณ ๋ฆฌ ๋ถํฌ๋ฅผ ๋ฐ๋ฅธ๋ค๊ณ  ํ๊ธฐํ  ์ ์๋ค. ๋์ด 2์ธ ์ฃผ์ฌ์๋ฉด์ด ๋์๋ค๊ณ  ํ ๋, ์ด๋ ์นดํ๊ณ ๋ฆฌ RV = [0,1,0,0,0,0]์ด ๋๋ค. RV์์ ๊ฐ ์์๋ค์ ๋ฒ ๋ฅด๋์ด ๋ถํฌ๋ฅผ ๋ฐ๋ฅด๊ณ , ๊ฐ๊ฐ ์์ ๋ค๋ง์ ๋ชจ์๋ฅผ ๊ฐ๋๋ค.

์นดํ๊ณ ๋ฆฌ๊ฐ K๊ฐ์ผ ๋, ์นดํ๊ณ ๋ฆฌ ๋ถํฌ์ ํ๋ฅ ์ง๋ํจ์๋ ์๋์ ๊ฐ๋ค.

<img src="..//images/sally/2021-05-01-23-49-44.png" width="50%">

<img src="..//images/sally/2021-05-01-23-46-12.png" width="50%">

> RV = Random Variable = ํ๋ฅ ๋ณ์

#### References

- [์นดํ๊ณ ๋ฆฌ ๋ถํฌ์ ๋คํญ๋ถํฌ - ๊ณ๋ํฌ์ ์คํ์ค](https://gem763.github.io/probability%20theory/%EC%B9%B4%ED%85%8C%EA%B3%A0%EB%A6%AC-%EB%B6%84%ED%8F%AC%EC%99%80-%EB%8B%A4%ED%95%AD%EB%B6%84%ED%8F%AC.html)
- [๊ฐ์๋จน๋ ํต๊ณ ๊ธฐ์ด1.ํ๋ฅ  ๋ถํฌ ์ ๋ฆฌ - ๊ฐ์๋จน๋ ๋จธ์ ๋ฌ๋](https://yeomko.tistory.com/33)

---

## #4

#### ๋คํญ ๋ถํฌ

์ฑ๊ณตํ๋ฅ ์ด ฮธ์ธ ๋ฒ ๋ฅด๋์ด ์ํ์ n๋ฒ ๋ฐ๋ณตํ์ ๋์ ์ฑ๊ณตํ์๊ฐ ์ดํญ๋ถํฌ๋ฅผ ๋ฐ๋ฅด๋ ๊ฒ์ฒ๋ผ, ์ฑ๊ณตํ๋ฅ ์ด <!-- $\theta=(\theta_1 ... \theta_k)$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=%5Ctheta%3D(%5Ctheta_1%20...%20%5Ctheta_k)">์ธ ์นดํ๊ณ ๋ฆฌ ์ํ์ n๋ฒ ๋ฐ๋ณตํ์ ๋์ ๊ฐ ์นดํ๊ณ ๋ฆฌ๋ณ ์ฑ๊ณตํ์๋ ๋คํญ๋ถํฌ(Multinomial distribution)์ ๋ฐ๋ฅด๊ฒ ๋๋ค.

<img src="../images/sally/2021-05-01-23-33-36.png" width="50%">

๋คํญ๋ถํฌ์ ์์์ ์๋์ ๊ฐ๋ค.

<img src="../images/sally/2021-05-01-23-43-27.png" width="60%">

> ์๋ฅผ๋ค์ด, ์ฃผ์ฌ์๋ฅผ 10๋ฒ ๋์ก์ ๋, 1์ด 1๋ฒ, 2๊ฐ 2๋ฒ, 3์ด 1๋ฒ, 4๊ฐ2๋ฒ, 5๊ฐ 3๋ฒ, 6์ด 1๋ฒ ๋์ค๋ ํ๋ฅ ์ ๊ณ์ฐํ๊ณ ์ ํ๋ค. ์ด๋ฅผ ๋ฒกํฐ๋ก ๋ํ๋ด๋ฉด (1, 2, 1, 2, 3, 1)์ด ๋๋ค. 6๋ฒ์ ๋์ก์ ๋ x๋ฒกํฐ์ฒ๋ผ ๋์ฌ ์กฐํฉ์ ๊ณ์ฐํด์ผํ๋ฉฐ, ์์์ ์๋์ ๊ฐ๋ค.

<img src="../images/sally/2021-05-01-23-52-20.png" width="40%">

#### References

- [์นดํ๊ณ ๋ฆฌ ๋ถํฌ์ ๋คํญ๋ถํฌ - ๊ณ๋ํฌ์ ์คํ์ค](https://gem763.github.io/probability%20theory/%EC%B9%B4%ED%85%8C%EA%B3%A0%EB%A6%AC-%EB%B6%84%ED%8F%AC%EC%99%80-%EB%8B%A4%ED%95%AD%EB%B6%84%ED%8F%AC.html)
- [๊ฐ์๋จน๋ ํต๊ณ ๊ธฐ์ด1.ํ๋ฅ  ๋ถํฌ ์ ๋ฆฌ - ๊ฐ์๋จน๋ ๋จธ์ ๋ฌ๋](https://yeomko.tistory.com/33)

---

## #5

#### ๊ฐ์ฐ์์ ์ ๊ท ๋ถํฌ

ํ๊ท ์ ์ค์ฌ์ผ๋ก ์ข์ฐ๊ฐ ๋์นญ์ธ ์ข ๋ชจ์์ ๊ทธ๋ฆฌ๋ ์ ๊ท๋ถํฌ์ด๋ค. ์ ๊ท ๋ถํฌ์ ํ๋ฅ  ๋ฐ๋ ํจ์์ ๊ทธ ๊ทธ๋ํ๋ ์๋์ ๊ฐ๋ค.  
<img src="../images/sally/2021-05-01-23-57-40.png" width="80%">  
<img src="../images/sally/2021-05-01-23-57-57.png" width="60%">

์ ๊ท ๋ถํฌ ์์์ ๋ณ์๋ <!-- $x$ --> <img style="transform: translateY(0.1em); background: white;" src="https://render.githubusercontent.com/render/math?math=x">์ด๋ค. ฯ์ ฮผ๋ ๊ทธ๋ํ๋ฅผ ์ข๋ชจ์์ผ๋ก ๋ง๋๋๋ฐ ์ฌ์ฉ๋๋ค. ฮผ๋ ํ๋ฅ  ๋ณ์ X์ ํ๊ท ์ด๊ณ  ฯ๋ํ๋ฅ  ๋ณ์ X์ ํ์ค ํธ์ฐจ์ด๋ค. ์ข ๋ชจ์์ ๊ทธ๋ํ๋ ํ๊ท ์ ๊ธฐ์ค์ผ๋ก ์ข์ฐ ๋์นญ์ ์ด๋ฃฌ๋ค. ํ์ค ํธ์ฐจ๊ฐ ๋์ ์๋ก ๊ทธ๋ํ๋ ์๋งํ ๊ณก์  ํํ๋ฅผ ๋๊ฒ ๋๋ค.

#### References

- [๊ฐ์๋จน๋ ํต๊ณ ๊ธฐ์ด1.ํ๋ฅ  ๋ถํฌ ์ ๋ฆฌ - ๊ฐ์๋จน๋ ๋จธ์ ๋ฌ๋](https://yeomko.tistory.com/33)

---

## #6

#### t ๋ถํฌ

t ๋ถํฌ๋ ์ ๊ท๋ถํฌ์ ๊ฐ์ด ์ค์ฌ์ ๊ธฐ์ค์ผ๋ก ์ข์ฐ ๋์นญ์ด๊ณ  ์ข๋ชจ์ ํํ๋ฅผ ๊ฐ๊ณ  ์ค์ฌ์ 0์ผ๋ก ๊ณ ์ ๋์ด ์๋ ๋ถํฌ์ด๋ค.

์์ ๋(degree of freedom, df)์ ๋ฐ๋ผ ์ข์ ํํ๊ฐ ์กฐ๊ธ์ฉ ๋ณํํ๋ค.

df๋ ํ๋ณธ์์ ๊ด๋ จ์ด ์๋ ๊ฐ๋์ผ๋ก, ํ๋ณธ์ด ๋ง์์ง๋ฉด ํ์ค์ ๊ท๋ถํฌ์ ๊ฑฐ์ ๋์ผํ ํํ๋ฅผ ๋ณด์ธ๋ค.

<!-- $Y \sim t(n)$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/fLtEVp8ASo.svg">์ด๋ฉด,
<br>
<!-- $f(y) = \frac{\Gamma\left(\frac{n+1}{2}\right)}{\Gamma\left(\frac{n}{2}\right)\cdot\sqrt{\pi n}}\cdot\left(\frac{n}{y^2+n}\right)^{\frac{n+1}{2}},\;\;\;-\infty < y < \infty$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/etNwUJGoHh.svg">
<br>
<!-- $E[Y] = 0\;\;\;Var[Y] = \frac{n}{n-2}$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/TZLEIjrSEx.svg">

> ๊ฐ๋ง ํจ์

<!-- $\Gamma(x) = \int_{0}^{\infty}u^{x-1}e^{-u}du$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/dFlfgEP1px.svg">

#### References

- [8.5 ์คํ๋ํธ t๋ถํฌ, ์นด์ด์ ๊ณฑ๋ถํฌ, F๋ถํฌ - ๋ฐ์ดํฐ ์ฌ์ด์ธ์ค ์ค์ฟจ](https://datascienceschool.net/02%20mathematics/08.05%20%EC%8A%A4%ED%8A%9C%EB%8D%98%ED%8A%B8%20t%EB%B6%84%ED%8F%AC,%20%EC%B9%B4%EC%9D%B4%EC%A0%9C%EA%B3%B1%EB%B6%84%ED%8F%AC,%20F%EB%B6%84%ED%8F%AC.html)
- [2.4 t-๋ถํฌ(t-distribution, Student's t-distribution) - Must Learning with R](https://wikidocs.net/34009)

---

## #7

#### ์นด์ด์ ๊ณฑ ๋ถํฌ

์ ๊ท ๋ถํฌ์ ์ ๊ณฑํฉ์ <!-- $\chi^2$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/HDjWnZkXVW.svg"> ๋ถํฌ๋ฅผ ๋ฐ๋ฅธ๋ค.
<br>

<!-- $Z \sim N(0, 1)\;\;\;\Rightarrow\;\;\;Z^2 \sim \chi^2(df=1)\;\;\;\Rightarrow\;\;\;\sum_{i=1}^{n}Z^2_i \sim \chi^2(df=n)$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/4FR6NRzuCY.svg">

#### References

- [8.5 ์คํ๋ํธ t๋ถํฌ, ์นด์ด์ ๊ณฑ๋ถํฌ, F๋ถํฌ - ๋ฐ์ดํฐ ์ฌ์ด์ธ์ค ์ค์ฟจ](https://datascienceschool.net/02%20mathematics/08.05%20%EC%8A%A4%ED%8A%9C%EB%8D%98%ED%8A%B8%20t%EB%B6%84%ED%8F%AC,%20%EC%B9%B4%EC%9D%B4%EC%A0%9C%EA%B3%B1%EB%B6%84%ED%8F%AC,%20F%EB%B6%84%ED%8F%AC.html)
- [2.5 ์นด์ด์ ๊ณฑ ๋ถํฌ์ F๋ถํฌ - Must Learning with R](https://wikidocs.net/34010)

---

## #8

#### F ๋ถํฌ

F ๋ถํฌ๋ ๋๋ฆฝ์ ์ธ <!-- $\chi^2$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/WGpBUWxpfr.svg"> ๋ณ์์ ๋น๊ฐ ๋ฐ๋ฅด๋ ๋ถํฌ์ด๋ค.
<br>

<!-- $Q_1 \sim \chi^2(n_1),\;\;\;Q_2 \sim \chi^2(n_2)\;\;\;\Rightarrow\;\;\;\frac{Q_1/n_1}{Q_2/n_2} \sim F(n_1, n_2)$ --> <img style="transform: translateY(0.1em); background: white;" src="../images/adc/deep-learning/1ushumHHBo.svg">

#### References

- [8.5 ์คํ๋ํธ t๋ถํฌ, ์นด์ด์ ๊ณฑ๋ถํฌ, F๋ถํฌ - ๋ฐ์ดํฐ ์ฌ์ด์ธ์ค ์ค์ฟจ](https://datascienceschool.net/02%20mathematics/08.05%20%EC%8A%A4%ED%8A%9C%EB%8D%98%ED%8A%B8%20t%EB%B6%84%ED%8F%AC,%20%EC%B9%B4%EC%9D%B4%EC%A0%9C%EA%B3%B1%EB%B6%84%ED%8F%AC,%20F%EB%B6%84%ED%8F%AC.html)
- [2.5 ์นด์ด์ ๊ณฑ ๋ถํฌ์ F๋ถํฌ - Must Learning with R](https://wikidocs.net/34010)

---

## #9

#### ๊ฐ๋ง ๋ถํฌ

๊ฐ๋ง ๋ถํฌ๋ **๊ฐ๋ง ํจ์**๋ฅผ ์ฌ์ฉํ์ฌ ์ ์ฒด **k๋ฒ์ ์ฌ๊ฑด**์ด ์ผ์ด๋  ๋๊น์ง **๊ฑธ๋ฆฌ๋ ์๊ฐ**์ ๋ํ๋ด๋ ์ฐ์ ํ๋ฅ ๋ถํฌ์ด๋ค.

theta ์ k ๋ ๊ฐ๋ง ๋ถํฌ์ ๋ชจ์์ด๋ค.

๊ฐ๋ง ๋ถํฌ๋ 0~๋ฌดํ๋๊น์ง ๊ฐ์ ๊ฐ์ง ์ ์์ผ๋ฉฐ ๋ชจ์์ ๋ฒ ์ด์ง์ ์ถ์ ์ ์ํด ์ฌ์ฉ๋๋ค.

<div align='center'>
<img src='../images/heath/gamma_dist_formula.png' height='100px'/>
</div>
<br>

<div align='center'>
<img src='../images/heath/gamma_dist.png' height='240px'/>
</div>
<br>

**๊ฐ๋ง ํจ์**  
**ํฉํ ๋ฆฌ์ผ**์ ํจ์๋ก ์ผ๋ฐํํ ๊ฒ

<div align='center'>
<img src='../images/heath/gamma_function.png' height='100px'/>
</div>
<br>

#### References

- [๊ฐ์๋จน๋ ํต๊ณ ๊ธฐ์ด [1] ํ๋ฅ  ๋ถํฌ ์ ๋ฆฌ - ๊ฐ์๋จน๋ ๋จธ์ ๋ฌ๋](https://yeomko.tistory.com/33)
- [8.7 ๋ฒ ํ๋ถํฌ, ๊ฐ๋ง๋ถํฌ, ๋๋ฆฌํด๋ ๋ถํฌ - datascience school](https://datascienceschool.net/02%20mathematics/08.07%20%EB%B2%A0%ED%83%80%EB%B6%84%ED%8F%AC,%20%EA%B0%90%EB%A7%88%EB%B6%84%ED%8F%AC,%20%EB%94%94%EB%A6%AC%ED%81%B4%EB%A0%88%20%EB%B6%84%ED%8F%AC.html)

---

## #10

#### ๋ฒ ํ ๋ถํฌ

๋ฒ ํ ๋ถํฌ๋ ๋ ๋ชจ์ a, b ์ ๋ํ **๋ฒ ํ ํจ์**๋ฅผ ๋ํ๋ด๋ ์ฐ์ํ๋ฅ ๋ถํฌ์ด๋ค.

๋ฒ ํ ํจ์๋ ์ดํญ ๊ณ์ (์กฐํฉ, combination ์ผ๋ก๋ ๋ถ๋ฆผ) ๋ฅผ ๋ํ๋ด๋ ํจ์์ธ๋ฐ, ์ดํญ ๊ณ์๋ ํฉํ ๋ฆฌ์ผ๋ก ์ด๋ฃจ์ด์ ธ์๊ธฐ ๋๋ฌธ์ ๋ฒ ํ ํจ์๋ ๊ฐ๋ง ํจ์๋ก ๋ํ๋ผ ์ ์๋ค.

๋ฒ ํ ๋ถํฌ์ ๊ฐ์ 0~1 ์ฌ์ด์ด๋ฉฐ ๊ฐ๋ง ๋ถํฌ์ ๋ง์ฐฌ๊ฐ์ง๋ก ๋ฒ ์ด์ง์ ์ถ์ ์ ์ํด ์ฌ์ฉ๋๋ค.

<div align='center'>
<img src='../images/heath/beta_dist_formula.png' height='100px'/>
</div>
<br>

<div align='center'>
<img src='../images/heath/beta_dist.png' height='240px'/>
</div>
<br>

#### References

- [๊ฐ์๋จน๋ ํต๊ณ ๊ธฐ์ด [1] ํ๋ฅ  ๋ถํฌ ์ ๋ฆฌ - ๊ฐ์๋จน๋ ๋จธ์ ๋ฌ๋](https://yeomko.tistory.com/33)
- [8.7 ๋ฒ ํ๋ถํฌ, ๊ฐ๋ง๋ถํฌ, ๋๋ฆฌํด๋ ๋ถํฌ - datascience school](https://datascienceschool.net/02%20mathematics/08.07%20%EB%B2%A0%ED%83%80%EB%B6%84%ED%8F%AC,%20%EA%B0%90%EB%A7%88%EB%B6%84%ED%8F%AC,%20%EB%94%94%EB%A6%AC%ED%81%B4%EB%A0%88%20%EB%B6%84%ED%8F%AC.html)

---
