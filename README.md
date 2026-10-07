# 🛒 Array Market

> Aprenda `map`, `filter` e `reduce` aplicando um cupom de desconto no seu carrinho.

**[▶ Ver ao vivo → map-filter-reduce-bice.vercel.app](https://map-filter-reduce-bice.vercel.app/)**

---

## 💡 A ideia

Explicações abstratas de `map`, `filter` e `reduce` costumam usar `[1, 2, 3]`. Aqui o aprendizado acontece num **marketplace experimental**: você recebe um carrinho com 6 produtos, revela um **cupom surpresa** e vê, passo a passo, cada método funcional transformando os dados.

Sem decorar sintaxe. Você vê o que cada função faz com algo que já conhece: preço, desconto e total.

## 🎮 Como funciona

A experiência é um pipeline em 5 etapas:

| Etapa | O que acontece |
| ----- | -------------- |
| 1. **Cupom** | Encontre e revele o cupom surpresa: **R$ 20 OFF** em cada produto |
| 2. **`map()`** | Cada produto vira uma nova versão com o desconto aplicado |
| 3. **`filter()`** | Só os produtos elegíveis (abaixo de R$ 200) continuam |
| 4. **`reduce()`** | Os preços restantes são somados em um total |
| 5. **Resultado** | Carrinho final: 6 produtos → 4 elegíveis → **R$ 355,00** |

Há também o **Modo Aula**, que faz perguntas e libera cada etapa só quando você está pronto.

## ✨ O código por trás

```js
produtosOriginais
  .map((produto) => ({ ...produto, preco: produto.preco - 20 }))
  .filter((produto) => produto.preco < 200)
  .reduce((total, produto) => total + produto.preco, 0);
```

- **`map()`** transforma os preços
- **`filter()`** seleciona os elegíveis
- **`reduce()`** calcula o total final

Três métodos, uma frase. Esse é o ponto.

## 🚀 Rodando localmente

```bash
# clone o repositório
git clone https://github.com/<seu-usuario>/map-filter-reduce.git

# entre na pasta
cd map-filter-reduce

# instale as dependências
npm install

# suba o servidor de desenvolvimento
npm run dev
```

Depois é só abrir o endereço que aparecer no terminal.

## 🛠️ Stack

- JavaScript
- Deploy na [Vercel](https://vercel.com)
- _(adicione aqui o framework e as libs que você usou)_

## 🤝 Contribuindo

Teve uma ideia de nova etapa, produto ou método (`find`, `some`, `every`...)? Abra uma *issue* ou mande um *pull request*.

## 📄 Licença

MIT. Use, estude, remixe.

---

<p align="center">
  <i>Simplicidade é a sofisticação máxima.</i>
</p>
