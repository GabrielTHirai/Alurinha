<h2>O que pensar ao utilizar o flexbox?</h2>

Primeiramente se analisa o que deve ser modificado, logo em seguida qual é o pai dos elementos em questão, com o pai definido, se aplica o flex na tag ou classe pai.
```
    display:flex;
```

No flexbox, existe uma propriedade que distribui o espaço entre os elementos, então ele pega o espaço inteiro e divide, caso tenha só 2 elementos, ele vai pegar e levar os 2 ao extremo (Tomar cuidado com essa propriedade, ja que vai ter vezes que ele não vai ter espaço para colocar ali, ai vai ter que recorrer à outras propriedades). Essa propriedade é o:
```
justify-content: space-between;
```

Para alinhar os elementos verticalmente, se usa:
```
align-items: center
```

Para dar um espaço em volta dos elementos:
```
justify-content: space-around
```

Para mudar a direção do flex (que naturalmente é em row(linhas)) para colunas, se usa:
```
    flex-direction: column;
```

Caso a página fique tudo junto, e sem quebrar nada, e você precise que ao final da página o flexbox pule pra baixo, se usa:
```
    flex-wrap: wrap;
```

Caso você tenha muitas classes definidas e queira pegar somente uma entre elas, você pode usar:
```
.conteudoPrincipal-cursos-link:nth-child(4)
```
Nesse caso ele vai pegar o 4 filho entre o conteudoPrincipal-cursos-link


Quando muda a direção do flex, para coluna, o align-itens : center faz ele centralizar ao centro horizontalmente e o justify-content: space-between muda de direção, antes ele separava os elementos que estavam no horizonte, agora ele vai separar verticalmente. é a ideia de main axis e cross axis.


Caso você queira mudar a ordem dos elementos, por exemplo, quero colocar um link primeiro que o outro, voce vai utilizar:
```
    order: -1;
```
por padrão o flex container vai vir com order 0, então se você quer mudar a order dos elementos, é só colocar um numero menor que todos.


Para entender melhor sobre o conceito de flexbox, segue o link:
```https://css-tricks.com/snippets/css/a-guide-to-flexbox/ ```

Uma propriedade que some com o espaço que sobrou e distribui entre os elementos, então se você coloca o flex grow em 2 itens de uma div, ele vai pegar e dividir entre eles pela proporção q colocar, se colocar 1-1, ele vai dividir em 2 somente, caso coloque mais ele vai dividindo igualmente.
```
flex-grow
```

ao diminuir o site, o elemento que tiver com essa propriedade, vai diminuir mais que o outro. Essa propriedade é o reverso do grow(podemos dizer assim).
```
flex-shrink: 2
```
<h3>OBS</h3>

Alguns navegadores não estão atualizados para o flexbox, como é o caso do "internet explorer", ja que essa é uma função nova e o navegador em questão é antigo.

caniuse.com (site para analisar se o navegador aceita uma propriedade ou não).