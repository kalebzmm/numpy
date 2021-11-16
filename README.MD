1. O que é Numpy?
2. O que fará o programa a seguir:
```python
import numpy as np
arr = np.array([-9, 1, 7], dtype=np.float32)
print(repr(arr))
```
3. Qual a diferença do programa da questão número para o programa a seguir:
```python
import numpy as np
arr = np.array([[10, 11, 12], [21, 22, 23]],
dtype=np.float32)
print(repr(arr))
```
4. Quando fazemos referencia a um array o que o Python faz? E qual a diferença para o copy?
```python
a = np.array([0, 1])
b = np.array([2, 3])
c = a
print('Array a: {}'.format(repr(a)))
c[0] = 99
print('Array a: {}'.format(repr(a)))

d = b.copy()
d[0] = -11
print('Array b: {}'.format(repr(b)))
```
5. O que faz a função astype (dê um exemplo)
6. Quando devemos usar np.nan?
7. Explique np.inf e -np.inf
8. Explique o funcionamento de arange
```python
arr = np.arange(5)
print(repr(arr))

arr = np.arange(5.1)
print(repr(arr))

arr = np.arange(-1, 4)
print(repr(arr))

arr = np.arange(-1.5, 4, 2)
print(repr(arr))
```
9. Faça um exemplo de códdigo com np.reshape
10. Para que serve np.transpose, np.zeros, np.ones, np.zeros_like, np.ones_like - aproveite e de um exemplo de cada em um programa

11. O que é aritmética multidimensional com python e de um exemplo de como usar

A aritimética multidimensional com Python possibilita realizar as operações básicas da matemática com arrays. Exemplo:
```python
arr1 = [1, 2, 3]
arr2 = [4, 5, 6]

print(np.multiply(arr1, arr2)) # Multiplica os valores dos dois arrays. Resultado: [4, 10, 18]
print(np.add(arr1, arr2)) # Soma os valores dos dois arrays. Resultado: [5, 7, 9]
print(np.subtract(arr1, arr2)) # Subtrai os valores dos dois arrays. Resultado: [-3, -3, -3]
print(np.divide(arr1, arr2)) # Divide os valores dos dois arrays. Resultado: [0.25, 0.4, 0.5]
```

12. Explique a linha de código abaixo da linha pontilhada no programa a seguir

```python
arr = np.array([[2, 4], [6, 9]])
# Imprime o exponencial de todos os valores dentro do array (e^x onde e = Número de Euler). Similar a 2.718281^2, 2.718281^4 ...
print(repr(np.exp(arr)))
# Imprime 2 elevado a cada um dos valores do array. Similar a 2^2, 2^4, 2^6, 2^9
print(repr(np.exp2(arr)))

arr2 = np.array([[1, 10], [np.e, np.pi]])
# Imprime o cálculo do logaritmo natural de cada valor do array. Atenção para np.e = Número de Euler, np.pi = valor de PI
# Similar a logₑ(1), logₑ(10)
print(repr(np.log(arr2)))
# Imprime o cálculo do logaritmo natural de cada valor do array com base 10 ao invés de e. Similar a log10(1), log10(10)
print(repr(np.log10(arr2)))
# Imprime 3 elevado a potência de cada item do array. Similar a 3^1, 3^10
print(repr(np.power(3, arr2)))
# Calcula x^2 onde x é o valor de cada item do array
print(repr(arr**2))
```
13. Como fazer a multiplicação de matrizes usando Numpy

```python
arr1 = [1, 2, 3]
arr2 = [2, 3, 3]

print(np.multiply(arr1, arr2)) # [2, 6, 9]
```
14. Por que usamos np.random.seed?
O np.random.seed faz com que os números "alteatórios" sejam previsíveis, ou seja, será mostrada sempre a mesma sequência de números ao utilizar o numpy.random.rand

15. O que faz e como funciona np.random.shuffle?
O np.random.shuffle embaralha um array. Exemplo:
```python
arr = [1, 2, 3, 4, 5]
np.random.shuffle(arr)
print(arr) # [4, 5, 1, 3, 2]
```

16. O que é uma distribuição "normal"?
```python
print(np.random.uniform())
print(np.random.uniform(low=-1.5, high=2.2))
print(repr(np.random.uniform(size=3)))
print(repr(np.random.uniform(low=-3.4, high=5.9,
size=(2, 2))))
```

17. Explique o programa usando as linhas pontilhadas
```python
arr = np.array([[0, 2, 3],
[1, 3, -6],
[-3, -2, 1]])
# .............................................
print(repr(arr == 3))
# .............................................
print(repr(arr > 0))
# .............................................
print(repr(arr != 1))
# .............................................
print(repr(~(arr != 1)))
```
18. Como somar e concatenar arrays
19. Como funciona np.save e np.load
20. Use as linhas pontilhadas para explicar
```python
arr = np.array([[0, 72, 3],
[1, 3, -60],
[-3, -2, 4]])
# .............................................
print(arr.min())
print(arr.max())
# .............................................
print(repr(arr.min(axis=1)))
# .............................................
print(np.mean(arr))
# .............................................
print(np.var(arr))
# .............................................
print(np.median(arr))

```