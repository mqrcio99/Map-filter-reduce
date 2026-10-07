# 🗺️ Map · Filter · Reduce

> Três funções. Infinitas possibilidades.

**[▶ Ver ao vivo → map-filter-reduce-bice.vercel.app](https://map-filter-reduce-bice.vercel.app/)**

---

## 💡 A ideia

`map`, `filter` e `reduce` são o trio que transforma loops confusos em código que se lê quase como uma frase. Este projeto existe para tornar essas três operações **visuais, interativas e fáceis de entender**.

Em vez de decorar a sintaxe, você vê os dados fluindo.

| Função   | O que faz                               | Entra → Sai          |
| -------- | --------------------------------------- | -------------------- |
| `map`    | Transforma cada item                    | `[1, 2, 3]` → `[2, 4, 6]` |
| `filter` | Mantém só o que passa no teste          | `[1, 2, 3]` → `[2, 3]`    |
| `reduce` | Junta tudo em um único valor            | `[1, 2, 3]` → `6`         |

## ✨ Em código

```js
const numeros = [1, 2, 3, 4, 5];

const resultado = numeros
  .filter((n) => n % 2 === 1)   // [1, 3, 5]
  .map((n) => n * 10)           // [10, 30, 50]
  .reduce((acc, n) => acc + n, 0); // 90
```

Sem `for`. Sem variável temporária. Só a intenção.

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

- Deploy na [Vercel](https://vercel.com)
- _(adicione aqui o framework e as libs que você usou)_

## 🤝 Contribuindo

Achou um bug ou teve uma ideia? Abra uma *issue* ou mande um *pull request*. Toda contribuição é bem-vinda.

## 📄 Licença

MIT — use, estude, remixe.

---

<p align="center">
  <i>Simplicidade é a sofisticação máxima.</i>
</p>
