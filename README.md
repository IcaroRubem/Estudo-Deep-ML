# Estudo-Deep-ML
Documentando meus estudos e aprendizados no [Deep ML](https://www.deep-ml.com/)

> Vector Operations
- Soma:
  `A soma dos índices correspondentes`
   
  $`\mathbf{u} + \mathbf{v} = (u_1 + v_1, u_2 + v_2)`$
  
  ```python
  def soma(u, v):
    return (a + b for a, b in zip(u, v))
  ```
- Produto Escalar:
  `A soma da multiplicação dos índices correspondentes`
  
  $`u \cdot v = \sum_{i=1}^{n}u_1v_1 =  u_1 \ast v_1 +...+ u_n \ast v_n`$

  ```python
  def produto_escalar(u, v):
    return sum(a * b for a, b in zip(u, v))
  ```
- Modulo
  `A raiz quadrada da soma dos quadrados dos valores`
  
  $`|u| = \sqrt{\sum_{i=1}^{n}u_i^2} = \sqrt{u_1^2 +...+ u_n^2}`$

  ```python
  from math import sqrt

  def modulo(u):
    return sqrt(sum(pow(a, 2) for a in u))
  ```

> Matrix Basics
- Transposição
  `Teste`

  ```python
  def transposicao(m):
  at = []

  i = 0
  for i in range(len(m[0])):
    s = []
    for d in m:
      s.append(d[i])
    at.append(s)

  print(at)
  ```
