# 📰 1º Prêmio de Jornalismo - Governo de Mato Grosso

Este repositório contém o código-fonte do site oficial do **1º Prêmio de Jornalismo do Governo de Mato Grosso**, desenvolvido com HTML5, CSS3, JavaScript e Bootstrap 5.  
O site é totalmente responsivo, com banners ilustrativos, botões interativos e um modal de inscrição funcional.

---

## 🚀 Tecnologias utilizadas

- **HTML5** — Estrutura semântica e acessível.  
- **CSS3** — Estilização moderna e responsiva.  
- **Bootstrap 5.3.3** — Sistema de grid e componentes.  
- **Font Awesome 6.5.2** — Ícones vetoriais.  
- **Google Fonts (Inter)** — Tipografia limpa e institucional.  
- **JavaScript (puro)** — Controle do modal, máscaras e validações.

---

## 🧩 Estrutura principal


---

## 🖼️ Principais seções do site

### 🟩 **1. Cabeçalho e navegação**
- Navbar fixa com links âncora para as seções principais.
- Ícone de acesso rápido à área administrativa.

### 🟨 **2. Banners institucionais**
Cada banner utiliza imagens distintas (`img/12.png`, `img/13.png`, `img/14.png`, etc.) com botões posicionados via CSS:
- `btn-banner12` → **Botão de inscrição**
- `btn-banner13` → **Botão do regulamento**
- `btn-banner14` → **Botão “Inscreva-se agora”**
- `btn-banner16` → **Botões duplos (Regulamento e Inscrição)**

Todos os botões foram convertidos para imagens clicáveis com ajuste responsivo.

### 🧾 **3. Modal de inscrição**
- Formulário de 3 etapas com validação dinâmica e barra de progresso.  
- Máscaras automáticas para **CPF** e **Telefone**.  
- Validação de campos obrigatórios antes do envio.  
- Suporte a upload de arquivos (PDF, JPG, MP4, MP3, ZIP).

### ⚙️ **4. Rodapé**
- Fundo com a imagem oficial (`img/17.png`).
- Informações de contato e ícones de redes sociais com hover animado.

---

## 📱 Responsividade

O layout foi cuidadosamente ajustado para:
- Desktop (≥1200px)
- Tablet (768–1024px)
- Mobile (≤768px)

Cada botão (`btn-banner12`, `btn-banner13`, etc.) possui posicionamento e redimensionamento dinâmico:
```css
@media (max-width: 768px) {
  .btn-banner13 {
    position: static;
    text-align: right;
    margin-top: -60px;
    padding-right: 12%;
  }

  .img-regulamento-link {
    width: 140px;
  }
}
