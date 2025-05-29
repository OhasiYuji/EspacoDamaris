
# Espaço Dâmaris - Landing Page

Esta é a landing page oficial do **Espaço Dâmaris**, uma empresa especializada em organização e mimos personalizados. O objetivo desta página é apresentar os serviços, produtos e valores da empresa, além de oferecer um canal de contato direto para potenciais clientes.

## 🚀 Funcionalidades

- **Design Responsivo:** O layout se adapta perfeitamente a diferentes tamanhos de tela (desktop, tablet, mobile), garantindo uma excelente experiência de usuário em qualquer dispositivo.
- **Navegação Fixa (Sticky Header):** A barra de navegação permanece visível no topo da página enquanto o usuário rola, facilitando o acesso às seções.
- **Menu Hambúrguer (Mobile):** Em dispositivos móveis, a navegação se transforma em um menu hambúrguer intuitivo, que se abre ao lado da logo e exibe os links verticalmente.

### Seções Informativas

- **Hero Section:** Introdução impactante com chamada para ação.
- **Sobre Nós:** Detalhes sobre a missão e a paixão do Espaço Dâmaris.
- **Serviços e Produtos:** Apresentação dos principais serviços e mimos oferecidos.
- **Depoimentos:** Prova social com feedbacks de clientes satisfeitos.
- **Chamada para Ação (CTA):** Incentivo para o contato.
- **Contato:** Informações de contato e um formulário para envio de mensagens.

### Outras Funcionalidades

- **Formulário de Contato Direto:** Utiliza a API do [EmailJS](https://www.emailjs.com/) para enviar e-mails diretamente para o seu e-mail sem a necessidade de um servidor backend próprio, com feedback de envio em tempo real.
- **Animações Suaves:** Efeitos de fade-in para elementos ao rolar a página.
- **Ícones Profissionais:** Utilização da biblioteca Font Awesome.
- **Scroll Suave:** Navegação suave entre as seções da página.

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estrutura semântica da página.
- **Tailwind CSS:** Framework CSS utilitário para estilização rápida e responsiva.
- **JavaScript:** Lógica de interatividade (menu hambúrguer, formulário de contato).
- **EmailJS:** Serviço de terceiros para envio de e-mails do frontend.
- **Google Fonts:** Utilização da fonte _Inter_ para tipografia moderna.
- **Font Awesome:** Biblioteca de ícones.

## ⚙️ Configuração e Uso

### Pré-requisitos

Para que o formulário de contato funcione corretamente, você precisa ter uma conta no [EmailJS](https://www.emailjs.com/) e ter configurado:

- Um Email Service (ex: Gmail, Outlook, SMTP).
- Um Email Template com os placeholders: `{{name}}`, `{{email}}`, `{{whatsapp}}`, `{{message}}`.
- Seu **Public Key (User ID)**, **Service ID** e **Template ID**.

### Instalação Local

1. Clone este repositório (ou baixe os arquivos diretamente).
2. Abra o arquivo `index.html` em seu navegador.

### Configuração do EmailJS no Código

No arquivo `index.html`, localize os seguintes trechos de código e substitua os placeholders pelos seus dados reais do EmailJS:

#### Public Key (User ID) - Inicialização do EmailJS:

```html
<script type="text/javascript">
  (function() {
    emailjs.init(""); // SEU Public Key (User ID)
  })();
</script>
```

**Substitua**: `ctPSw1a-ucwvQBXUB` pelo seu **Public Key (User ID)**.

#### Service ID e Template ID - Função de Envio do Formulário:

```js
const serviceID = "";   // SEU Service ID
const templateID = ""; // SEU Template ID
```

## 🌐 Publicação (Deploy)

Este é um site estático e pode ser facilmente hospedado em serviços como:

- **Netlify (Recomendado):** Basta arrastar e soltar a pasta do projeto ou conectar a um repositório Git.
- **Vercel:** Similar ao Netlify.
- **GitHub Pages:** Se você já usa o GitHub.
- **Firebase Hosting:** Uma opção robusta do Google.

## 📞 Contato

Para mais informações sobre o Espaço Dâmaris ou para solicitar um orçamento, entre em contato através do formulário na página ou pelos dados abaixo:

- **Telefone:** +55 31 99195-2216  
- **E-mail:** contato@espacodamaris.com.br

## ✨ Créditos

- Desenvolvido por **Yuji Ohashi**
- Ícones fornecidos por **Font Awesome**
- Tipografia do **Google Fonts**
- Funcionalidade de e-mail via **EmailJS**
