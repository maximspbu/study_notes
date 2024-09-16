---  
layout: mathjax  
---  
  
# 29. Понятие d-мерного линейного пространства $\mathbb{R}^d$, нормированного пространства, метрического пространства, примеры норм и метрик.  
  
### Примеры:  
$f(x,y)=x+y~-~\mathbb{R}^2$  
$f(x,y,z)=x\cdot y + z~-~\mathbb{R}^3$  
$f(x,y,z)=\begin{cases}  
x+y+z  
\\  
x-y-z  
\end{cases}\Leftarrow f:\mathbb{R}^3\to\mathbb{R}^2$  
  
### Обозначения:  
$\mathbb{R}^d=X;x\in X,$ где $x=(x_1,...,x_d)$ и $x_i\in \mathbb{R}$.  
$y\in\mathbb{R}^d\Rightarrow x+y=(x_1+y_1,...,x_d+y_d)$  
$\lambda x=(\lambda x_1,...,\lambda x_d)$  
$<x,y>=(x,y)=\displaystyle\sum_{k=1}^d x_k\overline{y_k},$ где $x_k,y_k\in\mathbb{C}$  
Если $X=\mathbb{R}^d$, то $y_k=\overline{y_k},$ так как $y_k\in\mathbb{R}$  
  
### Определение. Нормированное пространство, норма.  
$X~-~$линейное пространство, на котором задана функция:  
$||\cdot||:X\to\mathbb{R}$, называющаяся нормой, если $\forall x,y\in X$  
$1)$ $||x||\ge0$ и $||x||=0\Leftrightarrow x=0$.  
$2)$ $||\lambda x||=|\lambda|*||x||$, $\forall\lambda\in\mathbb{R}$  
$3)$ $||x+y||\le||x|| +||y||$  
Тогда пару $(X,||\cdot||)$ называют нормированным (евклидовым) пространством.  
  
### Примеры:  
$\boxed{1}$ $(\mathbb{R}^d,||\cdot||_p),$ где $p\ge1$.  
$x\in\mathbb{R}^d\Rightarrow||x||_p:=\Big(\displaystyle\sum_{k=1}^d|x_k|^p\Big)^\frac{1}{p}~-~$[нер-во Минковского](/www.notion.so/75-0a13e664fb124010b668e23d037c7d14?pvs=21).  
$\boxed{2}$ $p=\infty$  
$||x||_\infty=\displaystyle\max_{j\in1:d}|x_j|$  
  
$||x||_p\xrightarrow{p\to\infty}||x||_\infty$  
Попытка в доказательство:  
$\displaystyle||x||_p=\underset{p\to\infty}{\lim}\big[(\sum_{k=1}^d|x_k|^p)^\frac{1}{p}\le(d*\max(|x_k|)^p)^\frac{1}{p}=d^\frac{1}{p} \* \max(|x_k|)\big]=\\=\max(|x_k|)$  
  
$\boxed{3}$ $d\in C[a;b]=X$  
$||f||_C:=\displaystyle\max_{x\in[a;b]}|f(x)|~-~$равномерная норма.  
  
### Определение. Метрические пространства, метрика.  
$X~-~$линейное пространство.  
$\rho:X^2\to\mathbb{R}~-~$метрика, если выполняются аксиомы:  
$1)~\rho(x,y)\ge0$ и $\rho(x,y)=0\Leftrightarrow x=y$  
$2)~\rho(x,y)=\rho(y,x)$  
$3)~\rho(x,y)\le\rho(x,z)+\rho(z,y)$  
Тогда пару $(X,\rho)$ называют метрическим пространством.  
  
### Замечание.  
Если определена $||x||$, то $\rho(x,y):=||x-y||$ всегда метрика.  
  
### Пример.  
$\rho_p(x,y)=||x-y||_p=\displaystyle\big(\sum_{k=1}^d|x_k-y_k|^p\Big)^\frac{1}{p}$  
  
### Пример. Метрика, не определяемая нормой.  
$X=\mathbb{R}^1;\rho(x,y)=\dfrac{|x-y|}{1+|x-y|}~-~$метрика.  
$\rho(x,0)=\dfrac{|x|}{1+|x|}\ne||x||$  
$\rho(\lambda x,0)=\dfrac{|\lambda|\cdot|x|}{1+|\lambda|\cdot|x|}\ne|\lambda|\cdot\dfrac{|x|}{1+|x|}$  
