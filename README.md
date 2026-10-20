# Festival Despertacular · dados do app

Este repositório guarda a programação e os cartazes que o app **Festival Despertacular** (Android, `com.glc2.despertacular`) baixa quando abre.

- `programacao.json`: dias, atividades, sessões de filmes e atrações da festa.
- `cartazes/`: imagens (JPG, 800 px de largura).

Ao alterar e salvar aqui, os celulares recebem a mudança na próxima vez que o app abrir (pode levar alguns minutos).

## Avisos (pop-up)

No começo do `programacao.json` fica a lista `"avisos"`. Cada aviso aparece **uma vez** em pop-up quando a pessoa abre o app (versão 1.2 ou mais nova).

```json
"avisos": [
  {
    "id": "sala-19h",
    "titulo": "Mudança de sala",
    "texto": "A sessão das 19h de hoje será na sala 2.",
    "link": "",
    "botao_link": ""
  }
],
```

- `id`: um nome diferente para cada aviso. Se repetir um `id` já usado, quem já viu não vê de novo.
- `link` e `botao_link`: opcionais. Se tiver link, aparece um botão (ex.: "Comprar ingresso").
- Para tirar um aviso, apague o bloco dele. Para não ter aviso, deixe `"avisos": []`.
- Cuidado com as vírgulas: entre um aviso e outro tem vírgula; depois do último, não.

Os cartazes pertencem aos artistas e ao Festival Despertacular. Este repositório não concede licença de uso.
