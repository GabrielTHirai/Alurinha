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

<h3>OBS</h3>

Alguns navegadores não estão atualizados para o flexbox, como é o caso do "internet explorer", ja que essa é uma função nova e o navegador em questão é antigo.

caniuse.com (site para analisar se o navegador aceita uma propriedade ou não).