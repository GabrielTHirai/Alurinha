<h2>O que pensar ao utilizar o flexbox?</h2>

Primeiramente se analisa o que deve ser modificado, logo em seguida qual é o pai dos elementos em questão, com o pai definido, se aplica o flex na tag ou classe pai.

justify-content: space-between>>espaço entre os elementos. (Tomar cuidado com essa propriedade, ja que vai ter vezes que ele não vai ter espaço para colocar ali, ai vai ter que recorrer à outras propriedades)

align-items: center>>alinha verticalmente

justify-content: space-around>>espaço em volta dos elementos

    display: flex; 
    flex-direction: column; (serve para colocar o flex em colunas)
    flex-wrap: wrap;>> para quebrar a próxima coluna
.conteudoPrincipal-cursos-link:nth-child(4n){=====>>>>serve para pegar todo multiplo de 4, então todos elemento que são multiplos de 4 vai ter a margin zerada.
    margin-right: 0;
}

Quando muda a direção do flex, para coluna, o align-itens : center faz ele centralizar ao centro horizontalmente e o justify-content: space-between muda de direção, antes ele separava os elementos que estavam no horizonte, agora ele vai separar verticalmente. é a ideia de main axis e cross axis**

.cabecalhoPrincipal-nav-link-app{
    order: -1;
}>> por padrão o flex container vai vir com order 0, então se você quer mudar a order dos elementos, é só colocar um numero menor que todos.

https://css-tricks.com/snippets/css/a-guide-to-flexbox/ esse site ajuda muito a entender o flexbox.

flex-grow>>some com o espaço que sobrou e distribui entre os elementos, então se você coloca o flex grow em 2 itens de uma div, ele vai pegar e dividir entre eles pela proporção q colocar, se colocar 1-1, ele vai dividir em 2 somente, caso coloque mais ele vai dividindo igualmente.

flex-shrink: 2>>ao diminuir o site, o elemento que tiver com essa propriedade, vai diminuir mais que o outro. Essa propriedade é o reverso do grow(podemos dizer assim).

<h3>OBS</h3>

Alguns navegadores não estão atualizados para o flexbox, como é o caso do "internet explorer", ja que essa é uma função nova e o navegador em questão é antigo.

caniuse.com (site para analisar se o navegador aceita uma propriedade ou não).