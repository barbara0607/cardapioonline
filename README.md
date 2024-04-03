<!DOCTYPE html>
<head>
    <meta charset="UTF-8">
    <title>sua loja</title>
    <link href="estilo.css" type="text/css" rel="stylesheet">
    <style>
     /*
 * CSS Base
 */

/* Seleciona o corpo da pÃ¡gina */
body {

/** Muda a cor do fundo da pÃ¡gina **/
background-color: #e6e6e6;

/** Muda a fonte do corpo da pÃ¡gina e de todos os elementos
em seu interior para Candara, Helvetica (se Candara nÃ£o
estiver disponÃ­vel) ou uma fonte padrÃ£o sem serifa (se nem
Candara nem Helvetica estiverem disponÃ­veis) **/
font-family: Candara, Helvetica, sans-serif;    

/** Capaz de especificar  margens em elementos da pÃ¡gina
(partes superior, inferior, esquerda e direita). Alguns
elementos no HTML vem com margem embutida pelo navegador.
O corpo da pÃ¡gina Ã© um deles. Usando a definiÃ§Ã£o abaixo,
estamos removendo a margem de todos os lados do corpo da
pÃ¡gina, fazendo com que os elementos cheguem atÃ© as bordas
da mesma. Ã‰ possÃ­vel especificar valores de margem em px,
% e outras unidades de medida. TambÃ©m Ã© possÃ­vel especificar
a margem de forma individual, para cada lado do elemento
(margin-top, margin-right, margin-bottom e margin-left) **/
margin: 0;
}

/** Seleciona um elemento HTML com id definido para "header".
Em nossa pÃ¡gina, vai selecionar a div de cabeÃ§alho **/
#header {

/** Define a largura da div para que ocupe todo o espaÃ§o
disponÃ­vel do pai. No nosso caso, o pai Ã© o corpo da pÃ¡gina.
Portanto, a div de cabeÃ§alho ficarÃ¡ com a mesma largura
da pÃ¡gina **/
width: 100%;

/** Define uma altura fixa para a div de cabeÃ§alho. Nesse
caso, 137px **/
height: 137px;

/** Paddings sÃ£o utilizados para definir espaÃ§os ao redor de
elementos e atuam como uma "margem interna" (dentro da borda
do elemento). Nesse caso, estamos definindo um espaÃ§o de 
margem interna de 10px na parte superior da div **/
padding-top: 10px;
}

/** Seleciona a div que armazenarÃ¡ os elementos de logo (imagem
e texto do logo do site) **/
#logo {
/** Definimos uma largura capaz de armazenar a imagem e o texto
do logo do site. Neste caso, 340px **/
width: 340px;

/** Definimos uma altura capaz de armazenar a imagem e o texto
do logo do site. Neste caso, 100px **/    
height: 100px;

/** Desejamos posicionar esse elemento na pÃ¡gina, utilizando
elementos de posicionamento como left e top. Para que os mesmos
funcionem corretamente, Ã© necessÃ¡rio definir o tipo de
posicionamento como um valor diferente do padrÃ£o (static).
Utilizamos aqui o relative, jÃ¡ que o mesmo vai manter o espaÃ§o
reservado para os elementos do logo. Se usÃ¡ssemos o absolute,
perderiamos o espaÃ§o e os elementos que estÃ£o posicionados
logo abaixo do logo (menu) iriam "subir" e "encavalar" com o 
logo **/
position: relative;

/** Desejamos posicionar o logo no meio do pai (da div que ocupa
todo o espaÃ§o horizontal do corpo da pÃ¡gina. Para tanto, podemos
definir o posicionamento partindo da esquerda para a metade do
tamano do pai (50%) **/
left: 50%;

/** Como o posicionamento left considera o inÃ­cio do elemento
(parte mais a esquerda do mesmo) o posicionamento ficarÃ¡ "torto",
como se estivesse mais a direita do que deveria. Para corrigir
isso, precisamos adicionar uma "margem negativa" ao mesmo, removendo
metade de seu tamanho da esquerda. Desta forma, o elemento ficarÃ¡
corretamente posicionado ao meio. Como a largura do elemento foi
definida para 340px, a metade deste valor Ã© 170px. Sendo assim
definimos a margem do elemento para -170px. Esta tÃ©cnica pode ser
utilizada sempre que for necessÃ¡rio posicionar elementos no meio
da pÃ¡gina **/
margin-left: -170px;
}

/** Seleciona o elemento com o id "logoImg". No nosso caso, a imagem
que representa o logo do site**/
#logoImg {

/** O comando float faz com que elementos que normalmente
quebrariam linhas "flutuem" a esquerda ou a direita, nos
cantos do elemento pai onde se encontram. Ã‰ possÃ­vel flutuar
mais de um elemento, de forma que estes fiquem um ao lado do
outro. Estamos aplicando a fluaÃ§Ã£o na imagem e no texto do
logo, de forma que fiquem um ao lado do outro **/
float: left;
}

#tituloLogo {

/** O comando float faz com que elementos que normalmente
quebrariam linhas "flutuem" a esquerda ou a direita, nos
cantos do elemento pai onde se encontram. Ã‰ possÃ­vel flutuar
mais de um elemento, de forma que estes fiquem um ao lado do
outro. Estamos aplicando a fluaÃ§Ã£o  no texto de forma que o
mesmo fique ao lado da imagem **/
float: left;

/** Muda a cor do texto do logo **/
color: #4b4b4b;

/** Por padrÃ£o, usamos o elemento vertical-align: middle
para deixar elementos centralizados verticalmente. No entanto
Para elementos de texto, Ã© necessÃ¡rio definir o tamanho da linha
para o mesmo tamanho que se deseja que o texto fique no meio. A
propriedade line-height Ã© utilizada para tanto. Neste caso, estamos
configurando a linha para ter o mesmo tamanho da imagem, fazendo
com que o texto fique posicionado no meio desta **/
line-height: 100px;

/** Alguns elementos no HTML vem com margem embutida pelo
navegador, headers, por exemplo, jÃ¡ possuem valores de margem
prÃ©-estabelecidos. Usando a definiÃ§Ã£o abaixo,
estamos removendo a margem de todos os lados do h1 de tÃ­tulo,
fazendo com que o h1 fique posicionado corretamente, sem espaÃ§os
desnecessÃ¡rios **/
margin: 0;

/** Define o tamanho da fonte para 50px **/
font-size: 50px;
}

/** Seleciona a div principal que irÃ¡ compor o menu da aplicaÃ§Ã£o
(div com id = "menu") **/
#menu {

/** Define a largura da div para que ocupe todo o espaÃ§o
disponÃ­vel do pai. No nosso caso, o pai Ã© a div de header.
Portanto, a div de cabeÃ§alho ficarÃ¡ com a mesma largura
da div de cabeÃ§alho, que, atualmente, tem o tamanho pÃ¡gina **/
width: 100%;

/** Muda a cor do fundo da pÃ¡gina **/
background-color: #4b4b4b;
}

/** Seleciona a lista ordenada que compÃµe o menu **/
.listaMenu {

/** Definimos uma largura capaz de armazenar os itens de menu.
Neste caso, 340px **/
width: 300px;

/** Novamente, queremos posicionar a div na pÃ¡gina, utilizando
elementos de posicionamento como left e top. Para que os mesmos
funcionem corretamente, Ã© necessÃ¡rio definir o tipo de
posicionamento como um valor diferente do padrÃ£o (static).
Utilizamos aqui o relative, jÃ¡ que o mesmo vai manter o espaÃ§o
reservado para os elementos do menu. Se usÃ¡ssemos o absolute,
perderiamos o espaÃ§o e o elemento pai iria desaparecer, perdendo
a cor de fundo que atravessa a pÃ¡gina horizontalmente  **/
position: relative;

/** Novamente, vamos centralizar o elemento horizontalmente.
Para tanto, podemos definir seu posicionamento partindo da
esquerda para a metade do tamano do pai (50%) **/
left: 50%;

/** Novamente, vamos corrigir o posicionamento nÃ£o considerar o meio
do elemento, e sim o inÃ­cio (left) como cÃ¡lculo de posicionamento
percentual. Adicionamos uma "margem negativa", removendo
metade de seu tamanho da esquerda. O elemento ficarÃ¡
corretamente posicionado ao meio. Estamos utilizando um valor maior
que a metade do tamanho para compensar a margem que separa  os
elementos entre si **/
margin-left: -212px;

/** Definimos uma margem superior ao elemento, de forma que o
mesmo fique mais afastado do topo e, ao mesmo tempo,
centralizado **/
margin-top: 7px;
}

/** Seleciona todos os elementos de lista do item com a classe
"listaMenu" **/
.listaMenu li {

/** A propriedade display permite configurar como a disposiÃ§Ã£o
de elementos HTML Ã© feita na pÃ¡gina. Por padrÃ£o, elementos de
texto tem o display com o valor de "inline" (elementos sÃ£o
exibidos um ao lado do outro" e elementos de imagens, divs, e
etc tem o display configurado com display "block" (sÃ£o
posicionados de forma que ocupem um espaÃ§o vertical fixo, de
forma que outros elementos com display block caem para linha
de baixo). Abaixo, estamos utilizando o tipo especial de exibiÃ§Ã£o
denominado inline-block, que mistura os dois elementos. Elementos
com display inline-block sÃ£o organizados sequencialmente, uma ao
lado do outro, como texto, mas podem ter elementos de
dimensionamento e etc, como elementos em blocos.
Elementos display inline-block sÃ£o muito Ãºteis para transformar
listas verticais em elementos horizontais, muito Ãºteis em menus **/
display: inline-block;
}

/** Seleciona todos os links dentro de listas que estÃ£o dentro de
elementos com a classe "listaMenu" **/
.listaMenu li a {

/** Remove o sublinhado de links **/
text-decoration: none;

/** Configura o tamanho de 50px para os itens de link da lista **/
height: 50px;

/** Novamente, utilizamos o line-height para centralizar
elementos de texto verticalmente **/
line-height: 30px;

/** Utilizamos os elementos de padding para fazer com que
os itens de menu ganhem espaÃ§o horizontal (como botÃµes).
Isso ajuda a distanciÃ¡-los (caso contrÃ¡rio, ficariam grudados
horizontalmente uns nos outros) e, quando os links tiverem a
cor de fundo alterada para branco, parecerem "botÃµes". Estamos
definindo apenas as margens internas a esquerda e a direita, as
demais permanecem inalteradas **/
padding-left: 15px;
padding-right: 15px;
}

/** Seleciona elementos de link dentro de listas com a calsse
"listaMenu" quando estÃ£o em estado normal e quando estÃ£o
jÃ¡ visitados **/
.listaMenu li a:link,
.listaMenu li a:visited {

/** Muda a cor do texto dos links para branco **/
color: rgb(255, 255, 255);
}

/** Seleciona elementos de link dentro de listas com a calsse
"listaMenu" quando estÃ£o com o mouse apontado **/
.listaMenu li a:hover {

/** Muda a cor do link  **/
color: #4b4b4b;

/** Muda a cor de fundo para branco **/
background-color: rgb(255, 255, 255);
}

/** Seleciona os elementos com o id "menuAtual" quando em estado
normal e jÃ¡ visitados **/
#menuAtual:link,
#menuAtual:visited {

/** Utilizamos o item abaixo para deixar o texto em letra
maiÃºscula **/
text-transform: uppercase;

/** Deixa a fonte em negrito **/
font-weight: bold;
}

/** Selecionamos a div principal, que irÃ¡ armazenar todo o conteÃºdo
principal do site **/
#content {

/** Definindo um tamanho arbitrÃ¡rio para a div principal.
Neste caso, 700px. **/
width: 700px;

/** Definimos a cor branca para a div principal **/
background-color: white;

/** Usando o tipo de posicionamento junto ao left e ao margin
-left para centralizar a div principal horizontalmente na pÃ¡gina **/
position: relative;
left: 50%;
margin-left: -350px;
}

/** Selecionamos a div que contÃ©m os elementos de promoÃ§Ã£o **/
#promotionBanner {

/** Configura o tamanho de 200px para o banner promocional **/
height: 200px;

/** Configura uma imagem de fundo da promoÃ§Ã£o **/
background-image: url('images/promocao.jpg');
}

/** Seleciona o header principal da promoÃ§Ã£o (id "promocaoH1") **/
#promocaoH1 {

/** Define a cor da fonte como branca **/
color: white;

/** Define um tamanho de fonte de 64px; **/
font-size: 64px;

/** Remove a margem padrÃ£o dos elementos H **/
margin: 0;

/** Adiciona uma margem na esquerda do elemento, para "desgrudÃ¡-lo"
da borda lateral. Ã‰ possÃ­vel sobrescrever elementos de margem
definidos anteriormente combinando margin e margin-left, como aqui **/
margin-left: 20px;

/** Configura a posiÃ§Ã£o como absoluta, visando remover o espaÃ§o
reservado para o h **/
position: absolute;

/** Utilizado para definiÃ§Ã£o de sombra com CSS. O primeiro parÃ¢metro Ã©
o deslocamento horizontal da sombra, o segundo o vertical, o terceiro
a quantidade de blur a aplicar na sombra e o quarto a cor da mesma **/
text-shadow: 2px 2px 4px #4b4b4b;
}

/** Seleciona o header de valor da promoÃ§Ã£o (id "promocaoValor") **/
#promocaoValor {

/** Define a cor da fonte como branca **/
color: rgb(255, 255, 255);

/** Define um tamanho de fonte de 48px; **/
font-size: 48px;

/** Remove a margem padrÃ£o dos elementos H **/
margin: 0;

/** NecessÃ¡rio para poder posicionar os elementos **/
position: relative;

/** Utilizado para definiÃ§Ã£o de sombra com CSS. O primeiro parÃ¢metro Ã©
o deslocamento horizontal da sombra, o segundo o vertical, o terceiro
a quantidade de blur a aplicar na sombra e o quarto a cor da mesma **/
text-shadow: 2px 2px 4px #4b4b4b;

/** Posiciona o elemento no canto inferior direito **/
left: 180px;
top: 130px;

/** Restringe o tamanho padrÃ£o do H **/
width: 500px;
}


#tituloConteudo {
/** Define a cor do texto **/
color: #4b4b4b;
    
/** Alinha o texto do tÃ­tulo no centro **/
text-align: center;

/** Reduz a margem inferior padrÃ£o do H **/
margin-bottom: 10px;
}

/** Seleciona os elementos de tabela dentro da div com id
"areaProdutos" **/
#areaProdutos table {
/** Propriedade utilizada em tabelas para dar mais espaÃ§o entre cada
cÃ©lula **/    
border-spacing: 25px;

/** MantÃ©m os elementos de cÃ©lulas com margens entre elas **/
border-collapse: separate;

/** Alinha os elementos no centro da cÃ©lula por padrÃ£o **/
text-align: center;
}

/** Seleciona os elementos de td dentro da div com id
"areaProdutos" **/
#areaProdutos td {    

/** Configura uma largura padrÃ£o para cada cÃ©lula **/
width: 250px;

/** Configura uma cor padrÃ£o para o texto das cÃ©lulas **/
color: #4b4b4b;

/** Configura um tamanho de fonte padrÃ£o para o texto das cÃ©lulas **/
font-size: 20px;
}

/** Seleciona os elementos de imagem dentro de tds dentro da div com id
"areaProdutos" **/
#areaProdutos td img {

/** Configura um tamanho padrÃ£o para as imagens dos produtos **/
width: 150px;
height: 150px;

/** Separa a imagem do tÃ­tulo acima desta **/
margin-top: 5px;

/** Esta propriedade permite definir o quÃ£o arredondados os cantos
do elemento serÃ£o. 50% faz com que elementos que tem tamanho de altura
e largura iguais se tornem circulos **/
border-radius: 50%;

/** Permite especifiar a borda do elemento. O primeiro parÃ¢metro Ã© a
espessura da borda, o segundo Ã© o tipo da borda (solida, pontilhada, etc)
e o terceiro, sua cor **/
border: 2px solid #4b4b4b;
}

/** Seleciona elementos anotados com a classe "tituloProduto" **/
.tituloProduto {

/** Faz com que a fonte do elemento fique em negrito **/
font-weight: bold;

/** Remove a margem padrÃ£o dos elementos P **/
margin: 0;
}

/** Seleciona elementos anotados com a classe "precoProduto" **/
.precoProduto {

/** Remove a margem padrÃ£o dos elementos P **/
margin: 0;
}

/** Seleciona a div com o Ã­ncone e o telefone de entrega (id "entrega") **/
#entrega {

/** Configura o posicionamento como fixo. Desta forma, o elemento
ficarÃ¡ posicionado sempre relativo a Ã¡rea da tela do browser (viewport) **/
position: fixed;

/** Posiciona o elemento 30px em relaÃ§Ã£o a margem inferior **/
bottom: 30px;

/** Posiciona o elemento 10px em relaÃ§Ã£o a margem direita **/
right: 10px;

/** Define um tamanho para o elemento **/
height: 100px;
width: 300px;
}

/** Seleciona os elementos de imagem dentro elementos com id "entrega" **/
#entrega img {

/** Transforma o elemento num cÃ­rculo **/
border-radius: 50%;

/** Define uma borda para o elemento **/
border: 3px solid #4b4b4bd4;
}

/** Seleciona elementos com id "tel" **/
#tel {

/** Configura a posiÃ§Ã£o como absoluta, visando remover o espaÃ§o
reservado para o item e posicionÃ¡-lo arbitrariamente **/
position: absolute;

/** Configura uma posiÃ§Ã£o horizontal  para o item **/
left: 120px;

/** Define uma altura para o item **/
height: 75px;

/** Define a cor de fundo do item **/
background-color: #4b4b4b;

/** Define a cor do texto para branco **/    
color: rgba(255, 255, 255, 0.838);

/** Afasta o elemento do topo em 13px **/
margin-top: 13px;

/** Adiciona borda interna ao elemento no tamanho de 10px **/
padding: 10px;

/** Remove a borda interna da parte inferior  **/
padding-bottom: 0;

/** Arredonda um pouco os cantos da div **/
border-radius: 15px;
}

/** SeÃ§eciona os elementos h4 de um elemento com id "tel" **/
#tel h4 {

/** Remove as margens padrÃ£o do H **/
margin: 0;

/** Define um tamanho de fonte para o H4 em 28px **/
font-size: 28px;
}

/** SeÃ§eciona os elementos h5 de um elemento com id "tel" **/
#tel h5 {

/** Remove as margens padrÃ£o do H **/
margin: 0;

/** Adiciona uma pequena margem a parte superior do h5 **/
margin-top: 10px;
}

/** SeÃ§eciona os elementos a de um elemento com id "tel" **/
#tel a {

/** Define a cor do link como branco **/
color: rgba(255, 255, 255, 0.843);

/** Remove o underline do link **/
text-decoration: none;
}
    </style>
</head>
<body>
    <div id="header">
    <div id="logo">
    <img id="logoImg" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRukpmf4x303cnuP1pR5rCz2q7hYdgVohGdHGairI_wrZ8FDW_TMLbSEln8YsCjDfsmAfw&usqp=CAU">
    <h1 id="titulologo">Sua loja</h1>

    </div>
    <div>
        <div id="menu">
            <ul class="ListaMenu">
             <li><a href="sobre.html">Sobre Nós</a></li>
             <li><a id="menuAtual" href="index.html">Produtos</a></li>
             <li><a href="contato.html">Contato</a></li>
            </ul>
        </div>
        </div>

         <div id="content">
        <div id="promotionBanner">
            <h1 id="promoçãoH1">SUA PROMOÇÃO AQUI</h1>
        </div>
        <div id="maisVendidos">
            <h1 id="tituloConteudo">Produtos</h1>
            <div id="areaProdutos">
                <table>
                    <tr>
                        <td>
                            <p class="tituloProduto">x-Salada</p>
                            <img src="https://img.cybercook.com.br/receitas/151/x-salada-3.jpeg">
                            <p class="preçoProduto">R$19,00</p>
                            </td>
                            <td>
                                <p class="tituloProduto">Cheddar</p>
                                <img src="https://vixfrios.com.br/wp-content/uploads/2020/06/Cheddar-Cremoso.png">
                                <p class="preçoProduto">R$8,00</p>
                            </td>
                            </tr>
                            <tr>
                                <td>
                                    <p class="tituloProduto">Batata frita</p>
                                    <img src="https://cdn.casaeculinaria.com/wp-content/uploads/2023/03/13101208/Batata-frita.jpg">
                                    <p class="preçoProduto">R$15,00</p>
                                    </td>
                                    <td>
                                        <p class="tituloProduto">X-Burguer</p>
                                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTVDcS4Fky9MfGD7i0rLHgyX8iyLoG5blha6wvkqE1tN00rEbx2BAS8UKonqSxNu_6V3iU&usqp=CAU">
                                        <p class="preçoProduto">R$30,00</p>
                                    </td>
                                    <td>
                                        <p class="tituloProduto">Big Tower</p>
                                        <img src="https://www.baressp.com.br/eventos/fotos2/Big_Kahuna_02.jpg">
                                        <p class="preçoProduto">R$28,00</p>
                                        </td>
                                    </tr>
                                    <tr> 
                                        <td>
                                            <p class="tituloProduto">X-frango</p>
                                            <img src="https://s3-sa-east-1.amazonaws.com/deliveryon-uploads/products/traillerdoserginho/101_55afa6963dc16.png">
                                            <p class="preçoProduto">R$22,00</p>
                                        </td>
                                        <td>
                                            <p class="tituloProduto">Nuggets (c/8)</p>
                                            <img src="https://casadecarnesdomaninho.com.br/wp-content/uploads/2022/06/nuggtes.jpeg">
                                            <p class="preçoProduto">R$8,00</p>
                                        </td>
                                        <td>
                                            <p class="tituloProduto">Refrigerante (lata)</p>
                                            <img src="https://storage.googleapis.com/domain-images/0c38f198-2db6-46b9-a240-c94df814c742/products/gallery_05af6053-f2ee-42a1-b4d2-6ab32ae0f6fd.jpg">
                                            <p class="preçoProduto">R$4,00</p>
                                           </td>
                                           <td>
                                            <p class="tituloProduto">Sucos (vários sabores)</p> 
                                            <img src="https://www.receitasedicasdochef.com.br/wp-content/uploads/2020/12/Sucos-Naturais-Para-Hidratar-o-Corpo-e-a-Pele.jpg">
                                            <p  class="preçoProduto">R$4,00</p>
                                           </td>
                                                </tr>
                                                <tr>
                                                    <td>
                                                        <p class="tituloProduto">Pizza (de calabreza)</p>
                                                        <img src="https://p2.trrsf.com/image/fget/cf/1200/900/middle/images.terra.com/2023/07/10/dia-da-pizza-skkhweuqjcrq.jpg">
                                                        <p class="preçoProduto">R$25,00</p>
                                                        </td>
                                                        <td>
                                                            <p class="tituloProduto">Água (mineral)</p>
                                                            <img src="https://www.varanda.com.br/media/catalog/product/cache/1/image/1200x/9df78eab33525d08d6e5fb8d27136e95/a/g/agua-mineral-crystal-500ml-7894900530001.jpg">
                                                            <p class="preçoProduto">R$2,00</p>
                                                            </td>
                                                            <td>
                                                                <p class="tituloProduto">Paltel (c/caldo de cana)</p>
                                                                <img src="https://i0.wp.com/bernadetealves.com/wp-content/uploads/2021/12/Pastel-e-caldo-de-cana-combinacao-que-resiste-ao-tempo-e-movimenta-a-economia-Bernadete-Alves.jpg?fit=1200%2C645&ssl=1">
                                                                <p class="preçoProduto">R$25,00</p>
                                                                </td>
                                                                <td>
                                                                    <p class="tituloProduto">Salgados</p>
                                                                     <img src="https://www.sabornamesa.com.br/media/k2/items/cache/98401d211546397e2b8c04cfd4ec5a4d_XL.jpg">
                                                                     <p class="preço/produto">R$24,00</p>
                                                                     </td>
                                                                     </tr>
                                                                     </table>
                                                                     </div>
                                                                     </div>
                                                                     </div>
                                                                     
                                                                       <div id="entrega">
                                                                        <div id="tel">
                                                                            <a href="tel:555123456"></h4>(11)111-1111</h4</a>
                                                                            <h5>Entregamos 
                                                                            na sua casa</h5>
                                                                        </div>
                                                                        <img src="https://cdn-icons-png.flaticon.com/512/126/126341.png">
                                                                       </div>

                                                                    </body>

                                                             
--->
