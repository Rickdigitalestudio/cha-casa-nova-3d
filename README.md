# 🏠 Chá de Casa Nova — Lauane & Eduardo (versão 3D)

Convite interativo, dinâmico e em **3D** do chá de casa nova de **Lauane & Eduardo**.
Feito a partir do conteúdo do site original (Gamma) e reimaginado com Three.js — agora com
**casa própria, dois formulários funcionando dentro do site, endereço com mapa**.

## ✨ O que tem

- **Mansão 3D de dois pavimentos** construída em código: cozinha completa, sala, mesa de jantar,
  buffet de doces, canto de presentes, escadaria, quarto, escritório, banheiro, varanda com
  lounge e corda de luzes, cobertura de vidro flutuante — tudo em vidro, preto, branco e vermelho.
- **Jardim de festa**: gramado, caminho de pedras, cerca, árvores, canteiro com flores,
  balões, placa **147** e faixa **"NOVA CASA"** na entrada.
- **Câmera que viaja pelas seções** conforme você rola a página (10 enquadramentos com animação suave).
- **Arraste para girar** a casa, parallax com o mouse e deriva automática.
- **5 hotspots numerados** na cena que levam direto à seção correspondente.
- **Contador regressivo** até o dia do chá + **mapa do Google** embutido e link para navegação.
- **Formulário 01 — Lista de Presentes**: ~40 itens gerados (cozinha, mesa, sala, quarto, banheiro,
  casa geral) com reserva por nome, filtros por categoria e envio por WhatsApp.
- **Formulário 02 — Confirmação de Presença**: nome (com lista de 50 convidados), nº de pessoas,
  qual presente vai levar, mensagem, lista de confirmados e envio por WhatsApp.
- **Paleta de cores clicável** (vermelho, branco, preto, vidro) que muda o site **e** a cena 3D ao vivo.
- **Carrossel 3D** de utensílios (arraste ou setas) e **cards que viram 180°**.
- **Confete**, corações flutuando, tour automático, compartilhar no WhatsApp e copiar convite.
- **Responsivo** (desktop e celular) e **fallback 2D** automático se o WebGL não existir.

> Os dois formulários salvam as respostas no aparelho de quem preenche e montam a mensagem
> pronta para envio pelo WhatsApp (sem servidor). Assim funciona na hora, sem conta nenhuma.

## ✏️ Como editar data, endereço e links

Abra o `index.html` e ajuste o bloco `EVENTO` (início do primeiro `<script>`):

```js
const EVENTO = {
  data : '2026-11-22T16:00:00',   // data e hora reais do chá
  local: 'Rua Icatuaçu, 147 — Rio Grande da Serra/SP',
  mapa : 'https://www.google.com/maps/search/?api=1&query=...',   // botão "Abrir no Google Maps"
  mapaEmbed : 'https://www.google.com/maps?q=...&output=embed',  // mapa desenhado na página
  site : 'https://rickdigitalestudio.github.io/cha-casa-nova-3d/' // link usado no compartilhamento
};
```

Para trocar os itens da lista de presentes ou os nomes dos convidados, edite as listas
`PRESENTES` e `NOMES` no mesmo script (logo acima do bloco dos formulários).

## 🚀 Rodar localmente

Basta abrir o `index.html` no navegador, ou usar um servidor estático:

```bash
python -m http.server 8000
# http://localhost:8000
```

## 🌍 Publicar

Este repositório já publica automaticamente no **GitHub Pages**.
Qualquer alteração enviada para a branch `main` atualiza o site:

```bash
git add -A
git commit -m "Atualização"
git push
```

---

Feito com ❤ para Lauane & Eduardo.
