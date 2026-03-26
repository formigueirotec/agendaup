# 📅 Calendário UP — Unidade Popular

Interface web para exibição do calendário da sede da **Unidade Popular**, desenvolvida pelo **Núcleo de TI do MLC DF**.

---

## 🖼️ Visão Geral

Uma página web minimalista e responsiva que exibe o calendário semanal do Google Calendar da sede da Unidade Popular, com uma identidade visual sóbria e institucional (fundo escuro, efeito glassmorphism e imagem de fundo em escala de cinza).

---

## 🗂️ Estrutura de Arquivos

```
.
├── index.html                        # Estrutura HTML da aplicação
├── style.css                         # Estilização da página
├── UP.png                            # Logo da UP (versão clara — rodapé e favicon em modo escuro)
├── Logo UP Preto.png                 # Logo da UP (versão escura — favicon padrão)
└── 54987709272_f3f5ec4fc2_k.jpg     # Imagem de fundo
```

---

## ✨ Funcionalidades

- Exibição do calendário semanal via **Google Calendar Embed**
- Fuso horário configurado para **America/São_Paulo**
- Interface em **português brasileiro**
- Design com **glassmorphism** (fundo desfocado semitransparente)
- **Responsivo**: adapta o layout para telas menores que 1024px
- Favicons distintos para modo claro e escuro
- Link para o site oficial da Unidade Popular
- Crédito ao Núcleo de TI — MLC DF

---

## 🚀 Como Usar

Por ser uma aplicação puramente estática (HTML + CSS), não requer instalação de dependências ou servidor de build.

1. **Clone ou baixe** este repositório.
2. Certifique-se de que todos os arquivos estejam na mesma pasta:
   - `index.html`
   - `style.css`
   - `UP.png`
   - `Logo UP Preto.png`
   - `54987709272_f3f5ec4fc2_k.jpg`
3. Abra o `index.html` em qualquer navegador moderno.

> ⚠️ O calendário é carregado via `<iframe>` do Google Calendar e requer conexão com a internet para ser exibido.

---

## 🔧 Personalização

### Trocar o calendário exibido

No `index.html`, localize a tag `<iframe>` e substitua o valor do atributo `src` pela URL de incorporação do seu calendário do Google:

```html
<iframe
    src="SUA_URL_DO_GOOGLE_CALENDAR_AQUI"
    style="border-width:0"
    frameborder="0"
    scrolling="no">
</iframe>
```

Para obter a URL: **Google Calendar → Configurações do calendário → Integrar calendário → Incorporar código**.

### Trocar a imagem de fundo

Substitua o arquivo `54987709272_f3f5ec4fc2_k.jpg` pela imagem desejada e atualize a referência no `style.css`:

```css
#bg {
    background-image: url("NOME_DA_SUA_IMAGEM.jpg");
}
```

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML5 | Estrutura da página (`index.html`) |
| CSS3 | Estilização, glassmorphism, responsividade (`style.css`) |
| Google Calendar Embed | Exibição do calendário |

---

## 👥 Créditos

Desenvolvido pelo **Núcleo de TI — MLC DF**  
Site oficial: [unidadepopular.org.br](https://unidadepopular.org.br/)