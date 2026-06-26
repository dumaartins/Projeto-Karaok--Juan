# 🎤 Catálogo Karaokê — Rivo Trio

Catálogo digital de karaokê para shows da banda **Rivo Trio**. O público escolhe as músicas direto pelo celular, monta sua fila de pedidos e envia tudo via WhatsApp para a banda — sem necessidade de papel, fila física ou intermediário.

## ✨ Funcionalidades

- **Pop-up de boas-vindas** explicando como funciona o karaokê ao abrir a página.
- **Mais Pedidas** — seção em destaque com o ranking das músicas favoritas do público.
- **Catálogo por estilo musical**, organizado em abas:
  - 🇧🇷 Rock Nacional
  - 🖤 Emo / Punk
  - 🌿 Reggae
  - 🌎 Rock Internacional
  - 🎵 Pop, MPB & Festas
  - 🔥 Funk & Pop
- **Bandas expansíveis** — cada banda mostra sua lista de músicas ao clicar.
- **Fila de pedidos** — o usuário pode selecionar até 5 músicas por vez antes de enviar.
- **Envio via WhatsApp** — ao confirmar, o pedido (com nome do cantor e músicas escolhidas) é enviado automaticamente para o número da banda, formatado e pronto.
- **Área administrativa protegida por senha** — permite à banda adicionar novas músicas/bandas ao catálogo diretamente pela interface, sem precisar editar o código.
- **Visual escuro e responsivo**, com logo de fundo e identidade visual própria (paleta vermelho/dourado).

## 🛠️ Tecnologias

- HTML5
- CSS3 (puro, sem frameworks)
- JavaScript (vanilla)

Projeto 100% estático — não depende de backend, banco de dados ou build tools. Funciona abrindo o arquivo direto no navegador ou hospedando em qualquer servidor estático.

## 📁 Estrutura

```
.
├── index.html      # estrutura, estilos e lógica (tudo em um arquivo)
└── logo.png        # imagem de fundo/logo da banda
```

> Atualmente todo o código (HTML, CSS e JS) está em um único arquivo `index.html`. Pode ser separado em `style.css` e `script.js` futuramente, se desejado.

## 🚀 Como usar

1. Clone o repositório:
   ```bash
   git clone https://dumaartins.github.io/Projeto-Karaok--Juan/
   ```
2. Coloque a imagem `logo.png` na mesma pasta do `index.html` (usada como fundo da página).
3. Abra o `index.html` no navegador — não precisa de servidor nem instalação.

### Configurações importantes

No início do `<script>`, dentro do `index.html`, existem duas constantes que devem ser ajustadas conforme a necessidade da banda:

```javascript
const WHATSAPP_NUMBER = "5515996294176"; // número que recebe os pedidos
const ADMIN_PASS = "banda2025";          // senha da área administrativa
```

## 🎶 Como funciona para o público

1. Escolhe uma música do catálogo (ou das "Mais Pedidas").
2. Clica em **"Enviar"**.
3. Informa o nome.
4. O pedido é enviado automaticamente para o WhatsApp da banda.
5. Aguarda ser chamado para cantar!

## 🔧 Como a banda adiciona novas músicas

Na parte inferior do catálogo há uma seção **"Área da banda"**, protegida por senha. Após digitar a senha correta, é possível adicionar novas bandas/músicas a qualquer estilo, direto pela interface — sem precisar editar o código.

## 📄 Licença

Projeto de uso pessoal da banda Rivo Trio.
