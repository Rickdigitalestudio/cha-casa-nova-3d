# 🏠 Chá de Casa Nova — Lauane & Eduardo (versão 3D)

Convite interativo, dinâmico e em **3D** do chá de casa nova de **Lauane & Eduardo**.
Feito a partir do conteúdo do site original (Gamma) e reimaginado com Three.js.

## ✨ O que tem

- **Casa 3D interativa** construída em código (cozinha, sala, mesa de jantar, canto de presentes, parede e telhado de vidro) com sombras e reflexos.
- **Câmera que viaja pelas seções** conforme você rola a página (8 enquadramentos com animação suave).
- **Arraste para girar** a casa, parallax com o mouse e deriva automática.
- **5 hotspots numerados** na cena que levam direto à seção correspondente.
- **Contador regressivo** até o dia do chá.
- **Paleta de cores clicável** (vermelho, branco, preto, vidro) que muda o site **e** a cena 3D ao vivo.
- **Carrossel 3D** de utensílios (arraste ou setas) e **cards que viram 180°**.
- **Confete**, corações flutuando, tour automático, compartilhar no WhatsApp e copiar convite.
- **Responsivo** (desktop e celular) e **fallback 2D** automático se o WebGL não existir.

## ✏️ Como editar data, local e links

Abra o `index.html` e ajuste o bloco `EVENTO` (início do primeiro `<script>`):

```js
const EVENTO = {
  data : '2026-11-22T16:00:00',   // data e hora reais do chá
  local: 'Adicione aqui o endereço do chá',
  mapa : '',                       // link do Google Maps (opcional)
  form : 'https://docs.google.com/forms/d/e/.../viewform'  // lista de presentes / confirmação
};
```

## 🚀 Rodar localmente

Basta abrir o `index.html` no navegador, ou usar um servidor estático:

```bash
python -m http.server 8000
# http://localhost:8000
```

## 🌍 Publicar

Este repositório já publica automaticamente no **GitHub Pages**.
Qualquer alteração enviada para a branch `main` atualiza o site.

---

Feito com ❤ para Lauane & Eduardo.
