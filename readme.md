![GIF Site EDUC Bootstrap](https://github.com/Joaocosmala/Educ-Bootstrap/assets/78692465/4977cf2a-56b6-4d8f-bfc3-51e39c69382c)


## Site educacional desenvolvido com HTML e Bootstrap (Framework de CSS)
## Alguns ensinamentos básicos sobre Bootstrap para passar, assim ajudando a me conciliar da melhor forma na tecnologia, nos estudos, e com isso ajudando os demais. (Vale salientar que não sou nenhum profissional da tecnologia, muito pelo contrário, também sou estudante, e estou fazendo este README exatamente com o intuito de estudar, onde futuramente subirei o mesmo para o GITHUB, da onde você provavelmente está lendo este documento agora). Desde já agradeço chance e também a atenção!! Espero que aproveite e bons estudos!! #LetscodeDev

Estudos iniciante em Bootstrap - Por: João Cosmala.

Bootstrap - FrameWork de CSS - Linguagem de marcação para a estilização de páginas WEB.

Função - Estilizar páginas web dentro das classes no HTML
Exemplo: <div class="col-md-12 text-center mt-5">

Jajá explico o que cada um destes significa*

-----------------------------------------------------------------------------------------------------

Bootstrap trabalha inicialmente com sistema de GRIDS, que são nada mais do que linhas divisórias de toda a tela
Se iniciando do 1 e finalizando no 12, então imagine agora no seu monitor 12 linhas cortando de fora a fora entre top e bottom seu monitor,
esses são os famigerados GRIDs.

Com isso você trabalhará em todo o seu bootstrap para designar melhor aonde você pretende deixar cada conteúdo demonstrado, porém, isso tem de ser
feito sobre os 12 tipos de GRIDs.
Ou seja, a partir do momento em que você for alinhar algum elemento no seu FRONT-END, é de extrema importância que você saíba a melhor maneira
de fazer isso.



## GRIDS

- Se você tiver 4 elementos que vão ser colocados na tela de maneira alinhada, então terá que dividir estes GRIDs em:

Item 1: Item 2: Item 3: Item 4:
(1,2,3) (4,5,6) (7,8,9) (10,11,12)


- Se você tiver 3 elementos que vão ser colocados na tela de maneira alinhada, então terá que dividir estes GRIDs em:

Item 1:    Item 2:   Item 3:
(1,2,3,4) (5,6,7,8) (9,10,11,12,) 


- Se você tiver 2 elementos que vão ser colocados na tela de maneira alinhada, então terá que dividir estes GRIDs em:

Item 1:       Item 2:
(1,2,3,4,5,6) (6,7,8,9,10,11,12)


E por ai vai... Entendendo isso então você já vai ter pego a base de onde o Bootstrap se implementa.


-----------------------------------------------------------------------------------------------------

# Opções de grade - Pontos de interrupção.
# Xs - sm - md - lg - xl - xxl

Extra pequeno - (xs) - 576px
Pequeno - (sm) - 576px, 540px
Médio - (md) - 768px, 720px
Grande - (lg) - 992px, 960px
Extra grande - (xl) - 1200px, 1140px
Extra extra grande - (xxl) 1400px, 1320px

Extra pequeno - xs: Refere-se a dispositivos com uma largura de tela muito pequena, como smartphones em modo retrato. É o menor tamanho de tela considerado.
Pequeno - sm: Refere-se a dispositivos com uma largura de tela um pouco maior do que o xs, como smartphones em modo paisagem ou tablets em modo retrato.
Médio - md: Refere-se a dispositivos com uma largura de tela média, como tablets em modo paisagem ou monitores de tamanho moderado.
Grande - lg: Refere-se a dispositivos com uma largura de tela grande, como laptops e monitores de tamanho padrão.
Extra grande - xl: Refere-se a dispositivos com uma largura de tela extra grande, como monitores de alta resolução ou televisores.
Extra extra grande - xxl: Refere-se a dispositivos com uma largura de tela extremamente grande, como monitores de tela ampla.

O Bootstrap oferece classes CSS específicas para cada ponto de grade, assim permitindo que você defina o comportamento dos elementos
em diferentes tamanhos de tela. Por exemplo, você pode usar a classe col-xs-6 para definir uma coluna com metade da largura disponível
em dispositivos extra pequenos, enquanto a classe <class=col-lg-12> define uma coluna de largura total em dispositivos grandes.
Da primeira vez dá um nó na cabeça, mas depois que entende, fica simples.

Os pontos de grade são necessários pois eles permitem criar Layouts responsívos para a sua aplicação WEB, sempre se adaptando em todos os tipos de tela!!


# ROW
A Row é uma classe utilizada pra criar uma linha, ou seja, uma <row> dentro de um container organiza e alinha as colunas em um sistema responsivo.
Vale salientar novamente que: uma linha "row" é usada para agrupar colunas relacionadas horizontalmente, garantindo que as colunas se adequem de maneira
correta e se alinhem no espaço que estiver disponível a elas.

As colunas <Col-> devem sempre ser colocadas dentro de uma div com classe <row> para que o sistema de grade funcione corretamente.


# COL
No Bootstrap, a classe "col" é usada para criar colunas em um sistema de grade responsivo. 
sendo usada em conjunto com as classes relacionadas aos pontos de que logo veremos mais a fundo: 
"col-sm", "col-md", "col-lg", "col-xl" e "col-xxl", para definir o comportamento das colunas em diferentes tamanhos de tela.

Ou seja, a classe "col" é usada especialmente para criar uma coluna flexível para preencher o espaço disponível pelo conteiner pai.
A classe "col" pode ser combinada com outras classes para especificar como as colunas devem se comportar em diferentes pontos de grade. 
Por exemplo, "col-sm-6" define uma coluna que ocupa metade do espaço disponível em dispositivos pequenos ou maiores, enquanto "col-lg-8" 
define uma coluna que ocupa dois terços do espaço disponível em dispositivos grandes ou maiores que: 992px, 960px


# MD e MD-2
Exemplo: class"col-md-2" -> Estou dizendo que esta minha classe será "quebrada" ou seja, redimensionada quando minha tela chegar em 768px, para uma adaptação a outros dispositivos
Então, logo o 2 será a quantidade de grids que vão ser divididos para o meu conteúdo na tela, ou seja, 1,2,3,4,5,6 para o primeiro conteúdo e 7,8,9,10.11.12 para o segundo conteúdo, deixando a tela sendo ocupada na metade com um conteúdo de cada lado, como mostra o exemplo acima, em GRIDs.
Item 1:       Item 2:
(1,2,3,4,5,6) (6,7,8,9,10,11,12)


# Container-fluid (Acho legal já explicar isso por aqui)
Neste exemplo, o elemento <div> com a <class="container-fluid"> cria um contêiner de largura total. Você pode colocar seu conteúdo dentro deste contêiner e ele se expandirá para preencher toda a largura da janela do navegador.

<section>
    <div class="teste">
        <div class="container-fluid"> -> Container-Fluid para criar um container de largura total e responsivo com Bootstrap, fazendo seus itens se alinharem por todo o espaço de tela.
            <div class="row justify-content-center">
                <div class="col-md-4"> -> 4 GRID
                coluna1 (ocupando 1/4 do GRID)
                </div>
                <div class="col-md-4"> -> 4 GRID + 4 GRID = 8 GRID
                coluna2 (ocupando 2/4 do GRID)
                </div>
                <div class="col-md-4"> -> 4 GRID + 4 GRID + 4 GRID = 12 GRID
                coluna3 (ocupando 4/4 do GRID)
                </div>
            </div>
        </div>
    </div>        
</section>

No exemplo acima vemos nitidamente a estrutura de GRID na prática do que seria um código a utilizar os recursos de grid da melhor maneira.

Resumindo:

# ROW - Criar uma linha para o conteúdo em um sistema de grade responsivo
# COL - Criar colunas em um sistema de grade responsivo
# MD - Médio |.........
# MD-2 - Divisão de GRIDS em 2 com uma quebra em 768px

-----------------------------------------------------------------------------------------------------

# COLUNAS

<div class="row-align-items-start">
Alinhando todos os items no começo

<div class="row-align-items-center">
Alinhando todos os items no centro/meio

<div class="row-align-items-end">
Alinhando todos os items no final

-----------------------------------------------------------------------------------------------------

# TIPOGRAFIA (Tags para chamar texto em HTML)

<h1>
<h2>
<h3>
<h4>
<h5>
<h6>

Bom, se você já está estudando Bootstrap, provavelmente você já sabe como que funciona a questão das tags de texto em HTML5, porém, sempre vale ressaltar por aqui um conteúdo a mais para dar uma recordada a quem ainda está iniciando.

- Cada uma das TAGS, desde o h1 até o h6 irá definir um tamanho de texto para você utilizar em sua aplicação.
Partindo do h1 sendo o maior tipo, até o h6 sendo o menor tipo.

porém em Bootstrap você também pode chamar de maneira da qual preferir, e até mesmo de maneira separada.
Veja um exemplo:
<p class="h1">h1, Bootstrap</p>
<p class="h2">h2, Bootstrap</p>
<p class="h3">h3, Bootstrap</p>
<p class="h4">h4, Bootstrap</p>
<p class="h5">h5, Bootstrap</p>
<p class="h6">h6, Bootstrap</p>


Agora usando Display:

Caso o <h1> ainda não contente o tamanho preferivel de texto, temos em bootstrap o <display>, que também se origina a partir do 1 e até o 6 com a mesma grade de tamanho vista no <h1>, ficando assim bem fácil a compreensão.

<h1 class="display-1">display-1, Bootstrap</h1>
<h1 class="display-2">display-2, Bootstrap</h1>
<h1 class="display-3">display-3, Bootstrap</h1>
<h1 class="display-4">display-4, Bootstrap</h1>
<h1 class="display-5">display-5, Bootstrap</h1>
<h1 class="display-6">display-6, Bootstrap</h1>


-----------------------------------------------------------------------------------------------------


# Imagens

<img src="..........." class="img-fluid" alt="........">
Assim como com o HTML5 padrão usando uma tag de imagem para puxar uma imagem.
A class img-fluid define a img como fluída para se adaptar de acordo com qual a responsividade se altere.

<width> e <height> podem ser usados em sequência para definir uma largura e altura específica para a imagem.


-----------------------------------------------------------------------------------------------------


# Formulário EXEMPLO

<div class="card-body">
    <form class="row">
        <div class="col-md-6 mt-2"> - Definindo a coluna com um md de 6 para o grid e mt-2 (mt é espaçamento, como se fosse o Padding em CSS)
            <input type="text" class="form-control" placeholder="Nome Completo" aria-label="First name">
        </div>    
    </form>        
</div>

<input> = setando botão
<type="text"> = setando o tipo, que é texto
<class="form-control"> = setando o tipo de aparência para formulário em HTML, aplicando ajustes e estilos para melhorar a experiência do usuário
<placeholder="NomeCompleto"> = setando o conteúdo interno no holder do que é a atividade do botão
<aria-label="Firstname> = setando o conteúdo interno no holder do que é a atividade do botão


-----------------------------------------------------------------------------------------------------


# Cores e Botões

# Cores
<primary> - #Cor azul escuro
<secundary> - #Cor cinza
<success> - #Cor verde
<danger> - #Cor vermelha
<warning> - #Cor amarela
<info> - #Cor azul claro
<dark> - #Cor preto/cinza escuro

Cada uma das cores tem a intenção de passar uma emoção, com cada uma simbolizando algo, por isso os nomes.


# Botões
<class= btn btn-primary>
<class= btn btn-secondary>
<class= btn btn-success>
<class= btn btn-danger>
<class= btn btn-warning>
<class= btn btn-info>
<class= btn btn-light>
<class= btn btn-dark>

Os botões seguem a mesma linha que o restante de todos os processos em bootstrap, sendo utilizados quando puxado uma class e citando o tipo, <btn> e logo em seguida a sua estilização com <btn-primary> trazendo assim uma cor e uma intenção.


-----------------------------------------------------------------------------------------------------


# Função Card
O componente "card" é usado para criar contêineres flexíveis que podem exibir conteúdo relacionado, 
como informações, imagens, botões, etc. Os cards são úteis para organizar e apresentar informações de forma clara e visualmente agradável.

"CARD" em Bootstrap possui uma estrutura básica composta por uma div com a classe "card". Você pode adicionar conteúdo 
dentro do card usando outros elementos HTML, como cabeçalho, corpo, rodapé, etc. Para estilizar ainda mais o card, você pode adicionar classes adicionais ao componente.

<div class="card">
  <img src="imagem.jpg" class="card-img-top" alt="Imagem do Card">
  <div class="card-body">
    <h5 class="card-title">Título do Card</h5>
    <p class="card-text">Texto do Card que descreve o conteúdo.</p>
    <a href="#" class="btn btn-primary">Botão</a>
  </div>
</div>

Neste exemplo, temos um card simples com uma imagem no topo, seguida por um corpo de card
contendo um título, texto e um botão.
Você também pode adicionar outras classes ao componente "card" para personalizar seu estilo.
Por exemplo, você pode adicionar a classe "card-header" para criar um cabeçalho, a classe "card-footer" para adicionar um rodapé, e assim por diante.
Se passando assim exatamente como um "card" ou como podemos dizer em português "cartão".



-----------------------------------------------------------------------------------------------------



# Cores de FUNDO (BACKGROUND-COLOR)

Em bootstrap as cores de fundo também podem ser definidas através das classes que vimos anteriormente com success, primary e etc........
Assim, claro, podendo ser alteradas, porém, seguindo este como padrão.

<bg.primary>
<bg.secondary>
<bg.success>
<bg.danger>
<bg.warning>
<bg.info>
<bg.light>
<bg.dark>

O .bg significa = Background e a frente utilizamos a cor da qual queremos que seja passada.


# Opacidade

.bg-opacity-75 -> setando o nível de opacidade do background em 75%
.bg-opacity-60 -> setando o nível de opacidade do background em 60%
.bg-opacity-50 -> setando o nível de opacidade do background em 50%
.bg-opacity-44 -> setando o nível de opacidade do background em 44%
.bg-opacity-40 -> setando o nível de opacidade do background em 40%
.bg-opacity-10 -> setando o nível de opacidade do background em 10%


# Cores em textos com .text

Também podemos definir as cores das quais queremos utilizar somente em um texto específico, como por exemplo:
.text-primary -> ficando assim somente a cor azul em um texto único

<primary>
<secondary>
<success>
<danger>
<warning>
<info>
<light>
<dark>

E isso, novamente, podendo se repetir em todos os padrões de cores já estipulados pelo Bootstrap.

-----------------------------------------------------------------------------------------------------

# ESPAÇAMENTOS (MARGIN E PADDING EM BOOTSTRAP)

Margin sempre irá se distanciar de algum objeto que esteja próximo.
Padding sempre irá fazer um preenchimento em seu corpo levando também em consideração o outro objeto.

<m-2> -> Margem/Margin em relação à algum objeto. Se distância de algum objeto próximo.
<p-5> -> Padding = Preenchimento interno/expansão do próprio objeto.


tanto o <m> quando o <p> sempre iram ir de <1> a <5>
E este aumento é gradual levando em consideração o aumento anterior.
O bootstrap já deixa determinado um determinado espaçamento, ou seja, tanto m- quanto p- este não será alterado, pois o próprio framework já determinou no CSS um preenchimento específico.

Exemplo:

Margin
<m-1>
<m-2>
<m-3>
<m-4>
<m-5>

Padding
<p-1>
<p-2>
<p-3>
<p-4>
<p-5>

Top
<t-1>
<t-2>
<t-3>
<t-4>
<t-5>

Bottom
<b-1>
<b-2>
<b-3>
<b-4>
<b-5>

Ínicio
<s-1>
<s-2>
<s-3>
<s-4>
<s-5>

Fim
<s-1>
<s-2>
<s-3>
<s-4>
<s-5>

Para classes que definem -left e -right
<x-1>
<x-2>
<x-3>
<x-4>
<x-5>


Para classes que definem -top e -bottom
<y-1>
<y-2>
<y-3>
<y-4>
<y-5>


Exemplos práticos:

Em relação ao top
<mt-1>
<mt-2>
<mt-3>
<mt-4>
<mt-5>

Em relação ao bottom
<mb-1>
<mb-2>
<mb-3>
<mb-4>
<mb-5>

Em relação à left-right
<mx-1>
<mx-2>
<mx-3>
<mx-4>
<mx-5>

Em relação ao top e bottom
<my-1>
<my-2>
<my-3>
<my-4>
<my-5>

E como podem ver, nós podemos utilizar dos espaçamentos para qualquer direção que quisermos arquitetar nosso front.





# Text Positions 
<p class="text-start"></p>
<p class="text-center"></p>
<p class="text-end"></p>

Definindo as posições de um texto dentro de uma div/container

# Tamanhos em .fs e .fw para texto
.fs para textos funciona de maneira semelhante, se não igual, à questão dos h1,h2,h3,h4,h5,h6 e também display1, display2, display3, display4, display5, display6

Exemplo:
< fs-1 > tamanhos alternados
< fs-2 > tamanhos alternados
< fs-3 > tamanhos alternados
< fs-4 > tamanhos alternados
< fs-5 > tamanhos alternados
< fs-6 > tamanhos alternados

# FW - BOLDER
< fw-bolder > Deixa o texto em negrito (com peso e destaque)

# Icones de Bootstrap

O próprio site do bootstrap disponibiliza de maneira gratuíta acesso a uma galeria de ícones para uso em suas aplicações e estudos. Sejam elas acadêmicas ou profissionais.
Site abaixo linkado:
https://icons.getbootstrap.com/

Neste acesso ao bootstrap também é posto todas as informações mais detalhadas das quais estão aqui.
Assim como todo um tutorial de como usar e acesso a cópia de códigos já prontos em Bootstrap e HTML5 exatamente com o intuito de facilitar a produção de sites/aplicações web
favorecendo assim com uma maior produtividade e atividade. Facilitando o acesso e mantendo o Design para os seus códigos.
