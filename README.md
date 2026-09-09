# Vitrine Intellieng

Painel de aprovação das artes do Estúdio Autoral.

O Jhone abre no celular, aprova ou reprova cada peça e, ao reprovar, diz o motivo. As
decisões ficam no próprio aparelho e saem pelo botão "Copiar decisões para o Jarvis".

Gerado por `Maquina-de-Conteudo/11-Estudio-Autoral/publicar.py --web`, no repositório
`intellieng-cerebro`. Não edite `index.html` à mão: ele é sobrescrito a cada publicação.

## O que tem em `artes/`

Duas cópias de cada peça, nenhuma delas para postar:

| Arquivo | Para que serve |
|---|---|
| `<id>-mini.webp` | 560 px, é a que aparece na grade do catálogo |
| `<id>.jpg` | tamanho cheio, é a que aparece quando o Jhone amplia |

O original de postagem é o PNG, que o `entregar.py` copia para o ownCloud em
`Design Grafico › Estudio-Autoral › AAAA-MM-DD`. As duas cópias daqui são comprimidas
de propósito, para o painel abrir rápido no 4G da obra.

## Atualizar

```bash
cd Maquina-de-Conteudo/11-Estudio-Autoral
python3 publicar.py --web
bash subir-vitrine.sh
```
