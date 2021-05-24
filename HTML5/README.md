# BOX MODEL

Quando o browser renderiza uma página ele vai entender cada elemento como sendo uma caixa.
Cada caixa tem seu posicionamento, espaço, tem as suas propriedades.
Precisamos entender como funciona essas caixas

- Os elementos HTML são enxergados como caixas retangulares.

É composto de 4 partes, que definem um limite para o conteúdo (content);

1. Margin - (top, right, bottom, left)
2. Border - (top, right, bottom, left and style, width, color)
3. Padding - (top, right, bottom, left)
4. Conteúdo - (Content => texto, imagem, video)

Geralmente usamos a tag DIV como uma caixa que não é específica, que nos diz o que ela é. Temos por exemplo no html semantico as tags HEADER, MAIN, FOOTER, NAV, que nos diz o que elas são. A DIV geralmente não faz sentido, mas tem todas as propriedades de uma caixa como as tags semânticas.

## Padding
1. Quando adicionamos um padding-top de 100px, a caixa aumentou verticalmente;
2. Quando adicionamos um padding-left de 200px a caixa aumentou lateralmente;

Por que?
-Porquê ele somou os valores ao tamanho da caixa. Esse é um comportamento **padrão**

Para manter o tamanho inicial da caixa, eu tenho que dizer que o limite da caixa é fixo e que o preenchimento fique junto com o tamanho final da caixa.

**Como fazemos isso?**
- Inserimos uma propriedade chamada **box-sizing**

Agora observe que se adicionarmos um *padding-bottom: 500px;* a caixa vai aumentar. Isso se deve porque o tamanho adicionado é maior do que o limite da borda.


## Border 

Quando adicionamos a borda, ela altera o conteúdo, porém não aumenta o tamanho da caixa. Aqui ocorre o mesmo caso do **extrapolar o conteúdo**. Se tivermos uma borda muito grande ela pode fazer com que o conteúdo extrapole o tamanho da caixa, porém, **a caixa não aumenta de tamanho**.

As divs utilizadas, neste exemplo, tem como display padrão o **display: block;**.
Existem os **elementos de bloco** e os **elementos de linha**.
Nem todas as propriedades dos elementos em bloco, funcionam nos elementos em linha.
Você pode até converter um elemento em linha para um elemento **inliine-block**. Aí ele receberá normalmente as propriedades para bloco.
