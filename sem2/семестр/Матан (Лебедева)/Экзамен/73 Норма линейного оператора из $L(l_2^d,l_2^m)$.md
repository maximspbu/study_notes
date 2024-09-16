---  
layout: mathjax  
---  
  
# 73. Норма линейного оператора из $L(l_2^d,l_2^m)$  
  
### Следствие [теоремы](73 Норма линейного оператора из $L(l_2^d,l_2^m)$/72 Наибольшее и наименьшее значение квадратичной).  
$A\subset L(l_2^d,l_2^m)\Rightarrow\|A\|=\max\\{\sqrt{\lambda}~|~\lambda~-~$собственное число $A^TA\\}$  
  
### Доказательство:  
$A=\\{ a_{ij \\} }^{i=1,~\dots~,~m}_{j=1,~\dots~,~d};\quad A^T=\\{ a_{ji \\} }^{i=1,~\dots~,~m}_{j=1,~\dots~,~d}$  
  
$\displaystyle\|A\|^2=\sup_{|x|=1}|Ax|^2=\sup_{|x|=1}<Ax,Ax>~\stackrel{\text{Т. Вейерштрасса} }=\max_{|x|=1}<Ax,Ax>$  
  
$\displaystyle\stackrel{(a)}=\max_{|x|=1}<A^TAx,x>~\xRightarrow{Т}\max\\{\lambda~|~\lambda~-~$собственное число $A^TA\\}$  
  
### Примечание.  
Теорему Вейерштрасса можем применить, так как $S=\overline{B}\setminus B$, то есть [замкнутое - открытое = замкнутое](../Топология (Солынин)%20debeb4504e04449388d6167af66afe92/%D0%AD%D0%BA%D0%B7%D0%B0%D0%BC%D0%B5%D0%BD%20747e387df709426e8bb08555853c0343/5%20%D0%A0%D0%B0%D1%81%D0%BF%D0%BE%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5%20%D1%82%D0%BE%D1%87%D0%BA%D0%B8%20%D0%BE%D1%82%D0%BD%D0%BE%D1%81%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D0%BE%20%D0%BC%D0%BD%D0%BE%D0%B6%D0%B5%D1%81%D1%82%D0%B2%D0%B0%20%D0%B2%20%D1%82%D0%BE%D0%BF%D0%BE%20192c3d9104e64f0d9f759be954da42b5)  
  
### $\displaystyle(a):\quad<Ax,Ax>~=~<\Big(\sum_{j=1}^d a_{nj}x_j\Big)_{n=1}^m,\Big(\sum_{j=1}^d a_{nj}x_j\Big)_{n=1}^m>~=$  
  
$=\displaystyle\sum_{n=1}^m\Bigg(\Big(\sum_{j=1}^d a_{nj}x_j\Big)\Big(\sum_{j'=1}^d a_{nj'}x_{j'}\Big)\Bigg)=\sum_{n=1}^m\sum_{j=1}^d\sum_{j'=1}^d a_{nj}a_{nj'}x_j x_{j'}=$  
  
$=\displaystyle\sum_{j=1}^d\sum_{j'=1}^d\Big(\sum_{n=1}^m a_{nj} a_{nj'}\Big)x_j x_j'=~<A^TAx,x> ~~ \scriptsize\blacksquare$  
  
### Замечание.  
Если $a_{ij}\in\mathbb{C},$ то собственные значения $A^TA\in \mathbb{R}$.  
