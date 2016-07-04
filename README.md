# [Blogrid](https://andergtk.github.io/blogrid)

Grid CSS responsivo para sites com sidebar.

Se você tem um site que utiliza colunas com tamanho fixo nas laterais, esse
sistema de grid pode auxiliar você na organização desses componentes na sua
pagina.

## Instalar

Via [Bower](http://bower.io/)

```bash
bower install --save blogrid
```

Ou faça o [download ZIP](https://github.com/andergtk/blogrid/archive/v0.3.2.zip)
do repositório e copie o arquivo `blogrid.css` dentro da pasta do seu projeto.

## Configurar

Você deve adicionar a seguinte tag na seção `<head>` para não ter problemas com
a visualização em dispositivos móveis.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

E também *linkar* o arquivo do sistema de grid:

```html
<link rel="stylesheet" href="blogrid.css">
```

## Uso

Basicamente você precisa adicionar a classe `.grid` em cada *row* do seu site e
a classe `.col` em cada coluna.

As colunas do grid geral são nomeadas como frações (`.half`, `.one-third`,
`.one-fourth`, `.two-fifths`, etc).

Algumas classes não são necessárias como `.two-fourths` ou `.two-sixths` pois
existem outras equivalentes (`.half` e `.one-third`, respectivamente).

O sistema possui dois *breakpoints*, o primeiro é para telas com largura máxima
de `1300px`, que reduz a largura da classe `.container` que vem por padrão de
`1200px` para `1060px`, e o segundo *breakpoint* é com `960px`, que serve para
empihar as colunas em dispositivos menores.

Para evitar que as colunas fiquem empilhadas e com a largura total da tela, você
pode adicionar a classe `.no-stack` no `.grid` que manterá a largura padrão,
independente to tamanho de tela.

## Contribuindo

Se você tem alguma ideia e quer contribuir é só criar um
[pull request](https://github.com/andergtk/blogrid/pulls) ou abrir uma
[issue](https://github.com/andergtk/blogrid/issues).

## Licença

The [MIT License](LICENSE).
