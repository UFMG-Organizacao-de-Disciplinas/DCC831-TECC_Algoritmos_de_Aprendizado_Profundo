# Aprendizado Profundo - Professor Flavio Vinicius Diniz de Figueiredo - <flavio@dcc.ufmg.br>

## Comentários - 24/09/2024

- Façam 5 mini disciplinas.
- Requisitos
  - Álgebra
  - Cálculos 1 e 2
  - Probabilidade

- 100% focado no aprendizado profundo, sem o aprendizado clássico.

## Aula 3 - Perceptron

### Como viemos parar aqui?

Se você pega o assunto base, o resto vem fácil

- Primeira rede neural: perceptron
- ...

### Abordagem geral

- Comece com um problema simples, bem simples
  - Resolva o problema simples
- Como a solução do problema simples pode ser generalizada para problemas mais complicados?
  - Problema mais complicado = problema mais realista, mais próximo da realidade
- Problema simples:
  - Classificar objetos em DUAS classes: 0 ou 1
  - Problema linearmente serparável
    - Existe pelo menos uma linha reta que separa os dados das duas classes

SVM: o Algorítmo de SVM tenta achar a reta bem central com relação aos pontos mais no limite da borda entre os grupos.

Uma regressão logística tende mais pra média.
Hoje veremos qualquer reta simples que separe.
"O que é uma reta?"

Teremos muitas listas em Pytorch

### O que é uma reta?

- Entendendo uma reta:
  - O produto interno de um vetor com outro é zero quando são perpendiculares
  - $w.x=0$
  - $[1 0 1]*{[0 0 0]}^-1 = 0$
- A reta é definida por qualquer ponto acima da reta que defina um vetor cujo produto interno com w será zero.

$[w0 w1 w1] * {[1 y z]} = 0$
...
$y = -w0/w1 - (w2/w1)*x
$y = ax + b$

Somar uma constante em x1, altera nos eixos x; no x2 altera no y

### Hiperplano

### O problema

estudar o que é Sigmoid pra regressão logística; tem uma formuleta meio bizarra.
Ele falará sobre isso na próxima aula.

#### Abordagem geral do problema

- Problema simples:
  - Classificar objetos em duas classes: 0 ou 1
  - Problema linearmente separável
    - Existe pelo menos uma linha reta que separa os dados das duas classes

Kernel trick: uma forma de ir criando novas dimensões baseado na junção das variáveis das dimensões existentes. Um exemplo de visualização seria dispersar as as variáveis dispersas em outros eixos

### O algoritmo

Ao fazer cálculos com seno e cosseno conseguimos multiplicar isso para cada ponto, dessa forma, o sinal gerará a divisão entre as duas classes

### Interpretação geométrica

...

### Um monte de coisa

### Algoritmo do perceptron

```python

def perceptron (x: np.array, y: np.array, lambda: float [0,1)):
  X: shape[0]
  n = X*shape[0]
  X = ...
```

Já me perdi legal

Ao somar um vetor com um outro, isso já direciona o vetor para mais próximo de um deles

Em duas dimensões a reta vai subir e descer, mas em três dimensôes, o plano sempre passará pelo (0, 0, 0)

Complexidade: O(iterações * número de pontos * d alguma coisa)

### XOR Matador

### alguma coisa

### Prova do perceptron

Começa considerando que todos os pontos tem norma menor que R. Também se considera que existe uma reta.

### CAso quase linearmente separável

## Perguntar

## Aula 3 - Pergunta

- Falar sobre a geometria não euclidiana

## Estudar

### Aula 3 - Estudo

- [ ] Estudar o que é Sigmoid pra regressão logística; tem uma formuleta meio bizarra.
- [ ] Estudar Pandas e Numpy
- [ ] "Linear de distribuição sigma"
