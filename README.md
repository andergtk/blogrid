# Blogrid

Grid CSS responsivo para sites com sidebar.

Se você tem um site que utiliza colunas com tamanho fixo nos lados, esse sistema
de grid pode auxiliar você na organização desses componentes dentro da sua
pagina.

## Instalação

### Obtenha os arquivos

Através do gerenciador de pacotes [Bower](http://bower.io/)

```bash
bower install --save blogrid
```

Ou faça o [download zip](https://github.com/andergtk/blogrid/archive/master.zip)
do repositório e copie o arquivo `blogrid.css` dentro da pasta do seu projeto.

### Tags necessárias

Você deve adicionar a seguinte tag na seção `<head>` para não ter problemas com
a visualização em dispositivos móveis.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

E também linkar o arquivo do sistema de grid:

```html
<link rel="stylesheet" href="path/to/blogrid.css">
```

## Começando a utilizar

Adicione a classe `.grid` para cada *row* do seu template.

Adicione a classe `.col` em casa coluna do seu template.

As classes do grid geral estão nomeadas como frações (`.half`, `.one-third`,
`.one-fourth`, `.two-fifths`, etc).

**NOTA**: Algumas classes não são necessárias como `.two-fourths` ou
`.two-sixths` pois existem outras equivalentes (`.half` e `.one-third`,
respectivamente)

## Exemplos

#### Conteúdo + Sidebar

A sidebar tem a largura de 300 pixels por padrão e a largura do conteúdo é
ajustada automaticamente.

![](http://i.imgur.com/jhqQlje.png)

```html
<div class="grid">
	<div class="col content">
		<span>Content</span>
	</div>
	<div class="col sidebar">
		<span>Sidebar</span>
	</div>
</div>
```

#### Sidebar na esquerda + Conteúdo

![](http://i.imgur.com/3pCDqRc.png)

```html
<div class="grid">
	<div class="col content">
		<span>Content</span>
	</div>
	<div class="col sidebar-left">
		<span>Left sidebar</span>
	</div>
</div>
```

#### Conteúdo + Duas sidebars

![](http://i.imgur.com/Yv1jo17.png)

```html
<div class="grid">
	<div class="col content-two-sidebars">
		<span>Content with two sidebars</span>
	</div>
	<div class="col sidebar-left">
		<span>Left sidebar</span>
	</div>
	<div class="col sidebar">
		<span>Right sidebar</span>
	</div>
</div>
```

#### Grid geral

Você pode ver o código completo no arquivo `demo.html`.

![](http://i.imgur.com/iHO6vyM.png)

#### Empurrando colunas

Adicione a classe `.push-to-right` ou `.push-<fração>` para empurrar as colunas
até o local que você quer.

![](http://i.imgur.com/w0sDgk9.png)

#### Grids aninhados

Você pode fazer grids aninhados sem problemas, basta adicionar um novo `.grid`
dentro de uma coluna do grid pai.

![](http://i.imgur.com/eOirnga.png)

#### Espaço entre colunas (gutters)

Remova o espaçamento entre as colunas adicionando a classe `.no-gutters` no
`.grid`.

![](http://i.imgur.com/Bo7cYZu.png)

## Contribuindo

Se você tem alguma ideia e quer contribuir é só criar um [pull request](https://github.com/andergtk/blogrid/compare)
ou abrir uma [issue](https://github.com/andergtk/blogrid/issues/new).

## Licença

MIT License

Copyright (c) 2016 Blogrid
