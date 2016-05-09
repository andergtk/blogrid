# Blogrid

Grid CSS responsivo para sites com sidebar.

Se você tem um site que utiliza colunas com tamanho fixo nos lados, esse
sistema de grid pode auxiliar você na organização desses componentes na sua
pagina.

## Instalação

Através do gerenciador de pacotes [Bower](http://bower.io/)

```bash
bower install --save blogrid
```

Ou faça o [download zip](https://github.com/andergtk/blogrid/archive/master.zip)
do repositório e copie o arquivo `blogrid.css` dentro da pasta do seu projeto.

Você deve adicionar a seguinte tag na seção `<head>` para não ter problemas com
a visualização em dispositivos móveis.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

E também *linkar* o arquivo do sistema de grid:

```html
<link rel="stylesheet" href="path/to/blogrid.css">
```

## Começando a utilizar

Basicamente você precisa adicionar a classe `.grid` em cada *row* do seu site e
a classe `.col` em cada coluna.

As colunas do grid geral são nomeadas como frações (`.half`, `.one-third`,
`.one-fourth`, `.two-fifths`, etc).

Algumas classes não são necessárias como `.two-fourths` ou `.two-sixths` pois
existem outras equivalentes (`.half` e `.one-third`, respectivamente).

O sistema possui dois *breakpoints*, o primeiro é para telas com largura máxima
de `1000px` e o segundo com `800px`.

Para evitar que as colunas fiquem empilhadas e com a largura total da tela,
você pode utilizar a classe `.no-stack-ms` para não empilhar apenas no primeiro
*breakpoint* ou `.no-stack-never` que mantém a largura padrão do grid
independente da tela.

## Exemplos

Você pode ver o código completo no arquivo `demo.html`.

#### Conteúdo + Sidebar

A largura da sidebar tem `300px` e a do conteúdo é ajustada automaticamente.

![Imagem 1](http://i.imgur.com/SsibOcu.png)

```html
<div class="grid">
	<div class="col content">
		<span>Conteúdo</span>
	</div>
	<div class="col sidebar">
		<span>Sidebar</span>
	</div>
</div>
```

#### Sidebar na esquerda + Conteúdo

![Imagem 2](http://i.imgur.com/fYxbOJr.png)

```html
<div class="grid">
	<div class="col content">
		<span>Conteúdo</span>
	</div>
	<div class="col sidebar-left">
		<span>Sidebar na esquerda</span>
	</div>
</div>
```

#### Conteúdo + Duas sidebars

![Imagem 3](http://i.imgur.com/0sQa9iJ.png)

```html
<div class="grid">
	<div class="col content-with-sidebars">
		<span>Conteúdo com duas sidebars</span>
	</div>
	<div class="col sidebar">
		<span>Sidebar na direita</span>
	</div>
	<div class="col sidebar-left">
		<span>Sidebar na esquerda</span>
	</div>
</div>
```

#### Grid Geral

![Imagem 4](http://i.imgur.com/XAxSntb.png)

#### Empurrar Colunas

Adicione a classe `.push-to-right` ou `.push-<fração>` para empurrar as colunas
até o local que você quer.

![Imagem 5](http://i.imgur.com/8pU5fSb.png)

#### Grids Aninhados

Você pode fazer grids aninhados sem problemas, basta adicionar um novo `.grid`
dentro de uma coluna.

![Imagem 6](http://i.imgur.com/uGWsLTI.png)

#### Remover espaço entre colunas

Remova o espaçamento entre as colunas, que por padrão é de 20px, adicionando a
classe `.no-gutters` no `.grid`.

![Imagem 7](http://i.imgur.com/8pU5fSb.png)

## Contribuindo

Se você tem alguma ideia e quer contribuir é só dar um [pull request](https://github.com/andergtk/blogrid/compare)
ou abrir uma [issue](https://github.com/andergtk/blogrid/issues/new).

## Licença

The MIT License (MIT)
