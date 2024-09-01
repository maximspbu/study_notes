# 26. Исследование интеграла $\displaystyle\int_1^{+\infty}g(x)\sin(\lambda x)dx$

### Пример. Исследовать на сходимость $\displaystyle\int_1^{+\infty}g(x)\sin(x)dx$,
где $g$ монотонна и $g\ge 0$.

$1)$ $\displaystyle\int_1^{+\infty}g(x)$ сходится.
Тогда $|g(x)\sin(x)|\le|g(x)|=g(x)$
Отсюда по [признаку сравнения](../%D0%9A%D0%BE%D0%BD%D1%81%D0%BF%D0%B5%D0%BA%D1%82%D1%8B%203caed53170ce46dea253636711191f60/12%2003%2024%2039a2b45fc78441ed94f481ddc2ae2fe2.md):$\displaystyle\int_1^{+\infty}|g(x)\sin(x)|dx$ сходится,
а значит $\displaystyle\int_1^{+\infty}g(x)\sin(x)dx$ абсолютно сходится  $\tiny\blacksquare$

$2)$ $\displaystyle\int_1^{+\infty}g(x)$ расходится

$\quad 2.1)$ $\lim\limits_{x\to +\infty}g(x)=0$
Применим [признак Дирихле](../%D0%9A%D0%BE%D0%BD%D1%81%D0%BF%D0%B5%D0%BA%D1%82%D1%8B%203caed53170ce46dea253636711191f60/19%2003%2024%2089328aca7c30499d96e06881213e950d.md).
$|F(x)|=\Big|\displaystyle\int_1^x \sin(t)dt\Big|=\big|-\cos(t)|_{t=1}^x\big|=|\cos(1)-\cos(x)|\le
\\
\le|\cos(1)|+|\cos(x)|\le2\Rarr F$ ограничена.
Тогда $\displaystyle\int_1^{+\infty}g(x)\sin(x)dx$ сходится.

Рассмотрим $\displaystyle\int_1^{+\infty}|g(x)\sin(x)|dx$ и докажем, что он расходится.
$|\sin(x)|\ge\sin^2(x)=\dfrac{1}{2}-\dfrac{\cos(2x)}{2}$
Тогда $|g(x)\sin(x)|\ge\dfrac{g(x)}{2}-\dfrac{g(x)\cos(2x)}{2}$
Очевидно, что $\displaystyle\int_1^{+\infty}\dfrac{g(x)}{2}dx$ расходится (условие).
$\displaystyle\int_1^{+\infty}\dfrac{g(x)\cos(2x)}{2}=\dfrac{1}{4}\int_2^{+\infty}g\Big(\dfrac{t}{2}\Big)\cos(t)dt$ сходится по [признаку Д](../%D0%9A%D0%BE%D0%BD%D1%81%D0%BF%D0%B5%D0%BA%D1%82%D1%8B%203caed53170ce46dea253636711191f60/19%2003%2024%2089328aca7c30499d96e06881213e950d.md).

$\quad 2.2)$ $\displaystyle\lim_{x\to+\infty}g(x)\ne0$
Так как $g$ монотонна и $\ge0$, то $\displaystyle\lim_{x\to+\infty}g(x)=\alpha>0$.
Докажем, используя [критерий Коши](https://www.notion.so/4357e28572224d38bd413a03db3d2f6b?pvs=21), что $\displaystyle\int_1^{+\infty}g(x)\sin(x)dx$ расх.
Запишем отрицание [критерия Коши](https://www.notion.so/4357e28572224d38bd413a03db3d2f6b?pvs=21):
$\exist\varepsilon_0~~\forall b_0~~\exist b_1,b_2\in(b_0,+\infty):\Big|\displaystyle\int_{b_1}^{b_2}g(x)\sin(x)dx\Big|\ge\varepsilon$.
$\displaystyle\lim_{x\to+\infty}g(x)=\alpha\Rarr\exist A:\forall x\ge A:g(x)>\dfrac{\alpha}{2}$
$\sin(x)\ge\dfrac{1}{2}\Harr x\in\Big[\dfrac{\pi}{6}+2\pi k;\dfrac{5\pi}{6}+2\pi k\Big],k\in\Z$.
Возьмем $k:\dfrac{\pi}{6}+2\pi k\ge A$.
$\displaystyle\Big|\int_{\frac{\pi}{6}+2\pi k}^{\frac{5\pi}{6}+2\pi k}\underbrace{g(x)\sin(x)}_{\ge0}dx\Big|=\int \underbrace{g(x)}_{\ge\frac{\alpha}{2}}\underbrace{\sin(x)}_{\ge\frac{1}{2}}dx\ge\dfrac{2\pi}{3}\cdot\dfrac{\alpha}{2}\cdot\dfrac{1}{2}=\varepsilon_0~~\tiny\blacksquare$