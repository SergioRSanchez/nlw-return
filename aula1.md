Ao abrir nosso projeto, criamos o arquivo *index.html*. Clicamos com o botão direito do mouse e iniciamos o *Live Server*. Irá abrir uma página no Chrome que contém um **endereço de IP (Internet Protocol)** *(127.0.1)* e uma **porta** *(:5500)*. Portanto significa que ele fez um *servidor* usando nosso *endereço de IP*
**HTML**, ou Hyper Text Markup Language, é uma linguagem de marcação usando hyper textos.
**Figma** é uma ferramenta para quem desenha **interfaces**, ou seja, é uma ferramenta utilizada pelos **UI/UX** *(Usuary Interface/Usuary Xperience )*. Essa área é responsável para uma melhor *experiência* do usuário, como cores, fontes, localização dos itens...
Temos duas maneiras de usar imagens que estão no *Figma*, uma é utilizando o endereço do *svg* e outra é exportando o *png*. Outro serviço que temos de imagens é o <https://unsplash.com/>.
**Social Concern:** É muito importante por questões de acessibilidade, colocarmos uma *descrição* no *alt* da imagem, que aí o leitor de tela vai ler essa descrição para a pessoa.
Outro ponto interessante de colocar o *alt* na nossa imagem, é pois se procurarmos essa descrição no *Google*, será mostrada nossa página. Chamamos isso de **SEO** (Search Engine Optimization).

**CSS**, ou *Cascading Style Sheets*, é o responsável pelo estilo da página, a parte bonita que vemos.
**Social Concern:** Se usarmos o atributo *font-size* no *CSS* ele não deixa mudar a acessibilidade do nosso navegador, fica 'travado' aquele tamanho, pois o pixel é uma unidade *fixa*. Para evitarmos isso usamos o *REM*, que é uma unidade *relativa*. Para fazer isso, digitamos *:root {font-size: 100%;}* em nosso *style.css*, em que o padrão é de *16px*, aí para alcançar os *14px* de interesse, mudamos no *h4 {font-size: 0.8rem}*. Para ajudar nos cálculos, usamos o valor no root = 62.5% que é referente a 10px. Dessa maneira, fica formatado da maneira que queremos, e se alguém precisar usar a acessibilidade, poderá aumentar a fonte que ainda irá manter a formatação relativa.

Tudo que entendermos pos CSS e HTML são caixas, portanto tudo tem borda, altura, largura, espaços e por aí vai. No caso do nosso botão, ele é uma caixa com outra caixa dentro. Portanto **button é a tag pai** e o **svg é a tag filho**.

O *p*, o *h4*, o *h1* todos eles são um tipo de display do tipo **block**, que define que a caixa tem toda largura da página e ela sempre joga o próximo elemento pra baixo.

Já o *button* e *imagem* tem um tipo de display chamado **inline**, ou em linha, ele não pega toda a largura da página, e sim só o tamanho do próprio botão. Por isso, a princípio, as duas estão na mesma linha.

Alguns elementos são definidos como padrão pelo próprio navegador, por isso os espaços padrões que temos entre um bloco e outro. Se quisermos tirar tudo isso usamos um * { margin: 0; }. Isso fica visível se colocarmos uma borda colorida entre os elementos.

Toda caixa tem **conteúdo, altura, largura, preenchimento interno (padding), bordas, e espaço ao redor delas.**

Quando usamos o **display flex** mexemos com as tags filhas. Ele pega os elementos e coloca um do lado do outro, aí podemos alinhar o itens centralizados, justificar o conteúdo também como centralizados, e dar espaço entre os elementos. Lembre-se que quando usamos o flex, ele 'transforma' como se fosse um block, então temos que centralizar esse box.

Site para pegar fontes: <https://fonts.google.com/>

TERMINAR A PARTE DE BAIXO, VEJA QUE É UMA CAIXA, COM 3 CAIXAS DENTRO E 2 CAIXAS DENTRO DE CADA UMA DELAS. DICA É USAR O <DIV>

Para fazer a parte embaixo da imagem, vale observar que é um box com 3 box dentros, e dentro de cada box tem mais 2 box dentros. Para isso vamos usar **< div>** e colocar uma **classe**, que nada mais é que uma *propriedade/atributo universal* e serve para eu *classificar* um elemento.
No nosso caso a caixa maior vai ser a *class="stats"* e as menores dentro dela serão *class="stat"*.

Podemos usar o **short hand** do background ou de outras características, ou seja, *atalho*, nós usamos no *margin* passando dessa maneira ele coloca todos (left, right, bottom, top) com o mesmo valor.

O *display flex* a princípio coloca todos os itens um do lado do outro, mas podemos mudar sua **orientação**. No caso usamos orientação de *coluna*.

Nós mudamos a posição da imagem, e utilizamos *pixel*. Utilizamos pixel justamente pela acessibilidade, caso mexa na *font size*, a imagem continuará colada no box de baixo. Porém a imagem está mantendo o tamanho, independe do *"zoom"* que damos. Para corrigir isso mudamos a largura da imagem. Porém, agora mudando pela acessibilidade, a parte de baixo vai alterando, portanto temos que usar *rem* sim.

Iremos criar um *tag HTML* no nosso *CSS* Iremos fazer isso para criar um fundo em toda nossa *viewport*, e para isso usamos um unidade de medida que chama **vw (view width)**.

Agora vamos fazer o **menu**. Usamos uma caixa *nav* que é *navigation*. Ele tem que ficar fixo na página, então usamos o *position: fixed*. Porém ao fazer isso ele faz uma sobreposição de conteúdo.

Para fazer essa cor diferente do *menu* será usado **JavaScript**. O JavaScript é capaz de perceber movimentos que acontecem na página, portanto o *evento de rolagem* será percebido. Nós iremos colocar mais uma classe *(pode colocar mais de uma classe na mesma tag)* na nossa *tag nav*. Portanto, quando o JavaScript estiver rodando, ele mesmo vai colocar a *class scroll*.

Fazemos todo o processo de criar uma função de scroll e atribui-la ao nosso **id** do *navigate*.
Depois disso criamos uma lista **< ul>**.

Depois de vários passos que damos, vimos uma ferramenta de acessibilidade através da **aria css**.

Agora vamos para o Terceiro dia do nosso projeto. Hoje iremos colocar as caixas de referência dos nossos **serviços**. Temos uma caixa, que chamaremos de *header* também contendo *h4* e *h2*. Logo embaixo temos outra caixa que vai conter todos os **cards**, como se fossem *cartões*, que irão receber suas *configurações*.

Parei colocando 3 **card** dentro dos **cards**