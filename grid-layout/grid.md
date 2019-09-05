### Dicas Grid Layout

Para usar o grid, basta usar no estilo o `display: grid`

# Exemplo de usagem simples

```css
.container {
  display: grid;
  grid-template-columns: 100px auto 100px;
  grid-template-rows: 50px 50px;
  grid-gap: 3px;
}

/* É igual a... */
.container {
  display: grid;
  grid-template: repeat(2, 50px) / repeat(3, 1fr);
  grid-gap: 3px;
}
```

# Explicando código acima

Para a propriedade `grid-template-columns`, cada parametro é o comprimento da coluna.
Para a propriedade `grid-template-rows`, cada parametro é a altura da linha.
Extra: A propriedade `grid-gap` é o espaçamento entre os itens

Alguns dos parametros que as propriedades podem receber:

- `repeat(2, 50px)`
- `100px auto 1fr`

No primeiro container, o `grid-template` é a forma resumida dos
`grid-template-columns` e `grid-template-rows` onde o primeiro paramentro é as linhas
e o segundo as colunas.
