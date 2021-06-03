# Estudos sobre Flexbox

### 01/06/2021

# FLEXBOX

## Entendendo com o flexbox trabalha

- Flexbox trabalha com 2 eixos: main axis e cross axis;
- Existem propriedades para trabalhar com o **container** e propriedades para trabalhar com os **items**;
- Ao usar o **display:flex;**, por padrão, os elementos (flex-items) são organizados no **main axis**, da esquerda para direita;
- Se o container não tiver uma propriedade de tamanho especificada, ele ocupará a linha inteira;
- Se o container tiver uma **largura definida** e **dependendo da quantidade de items**, **eles poderão extrapolar o container**;
- Se definirmos uma altura para o container, por padrão, os *items* adotarão a altura do container;
- Dependendo da quantidade de `flex-items` que tiver dentro do seu container, eles poderão se expandir ou contrair, até que atinjam a largura máxima do container. E também os `flex-items` serão ajustados aos seus conteúdos.


### 02/06/2021

## flex-direction

- Por padrão, o *flex-direction* é definido como **row**.
- Ao modificar o *flex-direction* para **column**, invertemos o eixo principal para **cross axis** e o secundário para **main axis**.

### Valores para a propriedade flex-direction
1. row           -> Em linha, *da esquerda para direita*
2. row-reverse   -> Em linha, *da direita para esquerda*
3. column        -> Em coluna, *de cima para baixo*
4. colum-reverse -> Em coluna, *de baixo para cima*


## flex-wrap

- Define se os elementos `flex-items` do container irão quebrar a linha ou se irão continuar na mesma linha, mesmo que não caibam no seu container.
- Por padrão é definida com `no-wrap`.

### Valores para a propriedade flex-wrap
1. no-wrap      -> (sem quebrar linhas)
2. wrap         -> (quebra a linha se não os `flex-items` não couber na largura do container)
3. wrap-reverse -> (quebra a linha e colocando os `flex-items` no sentido inverso, ou seja, do **último elemento para o primeiro, da direita para a esquerda**.)