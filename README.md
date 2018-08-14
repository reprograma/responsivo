# Layout responsivo

* [Aula 1](#aula-1)
* [Aula 2](#aula-2)
* [Aula 3](#aula-3)

***

## Aula 1

#### O que é layout responsivo?

![responsive](https://media.giphy.com/media/b2CD0Qrq2ulwY/giphy.gif)

Hoje em dia temos uma enorme variedade de dispositivos onde um site pode ser visualizado (laptops, tablets, netbooks, celulares, desktops com tela pequena, iMacs com telas gigantescas, televisão, etc.). Seria inviável (e enlouquecedor) desenhar uma versão específica de um site para cada tamanho e resolução de tela disponíveis no mercado.

O design responsivo é uma das soluções para nos ajudar a resolver esse problema. Um layout responsivo que é aquele que se adapta ao diversos tamanhos de telas existentes. Ou seja, um mesmo layout que vai se adaptar desde a tela de celular até uma televisão de 42 polegadas.

A ideia do layout responsivo surgiu em 2010, com um designer chamado Ethan Marcotte
https://alistapart.com/d/responsive-web-design/ex/ex-site-flexible.html
https://alistapart.com/article/responsive-web-design


#### Alguns princípios do design responsivo:

* Adaptar o layout da página de acordo com a resolução em que está sendo visualizada;
* Redimensionar as imagens automaticamente para que caibam na tela e para que não sobrecarreguem a transferência de dados em um celular, por exemplo;
* Simplificar elementos da tela para dispositivos móveis;
* Ocultar elementos desnecessários nos dispositivos menores;
* Adaptar tamanho de botões e links para interfaces touch onde o ponteiro do mouse é substituído pelo dedo do usuário;
* Utilizar de forma inteligente recursos mobile como mudança na orientação do aparelho (horizontal ou vertical).

***

#### Porque layout responsivo é 😍  

* UX friendly: mantém o mesmo design adaptado para diferentes formatos de tela, sempre pensando na melhor usabilidade para cada formato;
* É mais barato desenvolver um site responsivo do que ter que desenvolver versões diferentes do site, em um versão mobile, por exemplo;
* É mais fácil dar manutenção, porque o código está todo em um lugar só (se tivesse uma versão mobile, por exemplo, uma mudança de código teria que ser feita em dois lugares);
* SEO friendly: como a aplicação só tem uma URL isso ajuda a manter todos os dados consistentes e a melhorar a posição no ranking do Google.

***

#### Porque layout responsivo é 🤦‍

![Mockup](images/devices.png)

* Versões antigas do IE;
* Se o layout e a arquitetura do código não forem desenhadas antes de começar o trabalho, o site pode ficar muito difícil de manter/modificar;
* O site responsivo pode ser mais demorado de carregar (se tiver muitas imagens redimensionadas, por exemplo);


#### Resolução de tela x tamanho de tela

Resolução de tela: A resolução da tela de um dispositivo é o número de pixels em cada dimensão que podem ser exibidos.

Tamanho de tela: tamanho físico da tela, normalmente medido em polegadas

Dispositivos com o mesmo tamanho podem ter resoluções de tela diferentes (Exemplo: iPhone 3 e 4)

http://teknosrc.com/resolution-vs-pixel-density-in-displays-all-you-need-to-know/

https://fueled.com/blog/iphone-screen-size-screen-resolution/


#### Quando vale a pena ter um site com:

* Layout responsivo
* Versão mobile/tablet
* App nativo

***

#### Técnicas de layout responsivo que vamos aprender

1) Grid fluido: Uso de % ao invés de valores absolutos (px)
https://alistapart.com/article/fluidgrids

2) Media queries: São breakpoints que modificam o CSS para cada resolução de tela.
https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries

***

#### Vamos começar?

O primeiro passo é adicionar a metatag viewport  no <head> do site. Essa tag vai passar instruções para o browser renderizar o conteúdo conforme o tamanho do dispositivo.


<meta name="viewport" content="width=device-width, initial-scale=1">

```
@media (max-width: 768px) {
   color: #fff;
}
```

`Se [largura do dispositivo] for menor ou igual a 768px, então execute o {...}`

```
@media (min-width: 768px) {
   color: #fff;
}
```
"Se [largura do dispositivo] for maior ou igual a 768px, então execute o {...}"

```
@media (max-width: 768px) and (min-width: 600px) {
   color: #fff;
}
```
`Se [largura do dispositivo] for entre 768px e 600px, então execute o {...}`

Apesar da grande variedade de dispositivos disponíveis no mercado, existem alguns breakpoints padrões que são mais usados:

```
1280px
1024px
768px
320px
```

* [Exercicio - Transformar um layout feito para desktop em responsivo](https://github.com/reprograma/responsivo/tree/master/exercicio-desktop-para-responsivo)


***

## Aula 2

#### Como testar?

#### Font-size responsive

#### Imagens responsivas

#### JPG, PNG e SVG

Quando você salvar

* [Exercicio - Codar um layout responsivo do zero](https://github.com/reprograma/responsivo/tree/master/exercicio-responsivo-do-zero)

***

## Aula 3

#### Mobile first

O que é mobile first?
É exatamente o que o nome sugere: pensar em toda a estrutura de um site a partir do mobile e depois ir progressivamente pensando nas telas maiores.

***

#### Porque é importante

![Mockup](images/mobile-first-1.png)
![Mockup](images/mobile-first-2.png)
![Mockup](images/mobile-first-3.png)


Apesar do número de usuários que acessam sites pelo celular/tablet, é mais comum para os designers/desenvolvedores pensar no site a partir do desktop, que é a tela que eles estão olhando quando estão trabalhando. Depois de tudo pensando para desktop, começa um processo de “aperta pra caber” o conteúdo no mobile


Só que nesse processo alguma informação importante para o usuário que acessa pelo celular pode ser cortada do site, e outras informações não tão relevantes podem ser mantidas.


Porque mobile first é 😍

* A maior vantagem desse método é a otimização do site para o celular, com foco em conteúdo e funcionalidade para melhorar a experiência do usuário


Porque mobile first é 🤦‍

* No processo de pensamento minimalista você pode acabar perdendo boas ideias

* [Exercicio - Codar um layout mobile first](https://github.com/reprograma/responsivo/tree/master/exercicio-mobile-first)
