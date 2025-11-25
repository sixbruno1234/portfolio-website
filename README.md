# Portfólio Profissional - Desenvolvedor Web & IA

Site de portfólio moderno e profissional criado para freelancers que trabalham com desenvolvimento web e inteligência artificial.

## Características

- Design dark mode profissional
- Totalmente responsivo (mobile, tablet, desktop)
- Animações suaves ao scroll
- Navbar com efeito blur ao scroll
- Seções completas: Hero, Sobre, Projetos, Serviços, Contato
- Formulário de contato com validação
- Integração com WhatsApp
- SEO otimizado
- Performance otimizada

## Tecnologias Utilizadas

- HTML5
- Tailwind CSS (via CDN)
- JavaScript Vanilla
- Font Awesome Icons
- Google Fonts (Inter & Poppins)

## Estrutura do Projeto

```
portfolio-website/
├── index.html          # Arquivo principal
├── assets/
│   └── images/         # Pasta para suas imagens personalizadas
└── README.md           # Este arquivo
```

## Como Personalizar

### 1. Informações Pessoais

Abra o arquivo `index.html` e personalize:

- **Linha 17-19**: Meta tags (description, keywords, author)
- **Linha 24-25**: Open Graph tags para redes sociais
- **Linha 124**: Logo/nome no navbar (`&lt;DevAI/&gt;`)
- **Linha 160-165**: Título principal da seção Hero
- **Linha 167-169**: Subtítulo da seção Hero

### 2. Estatísticas (Hero Section)

Linhas 186-198: Ajuste os números conforme seu perfil

```html
<p class="text-3xl font-bold gradient-text">16</p>
<p class="text-sm text-gray-400">Anos de Idade</p>
```

### 3. Seção Sobre

- **Linhas 226-245**: Edite o texto sobre você
- **Linhas 251-297**: Ajuste as habilidades técnicas (adicione ou remova tags)

### 4. Projetos

Linhas 315-490: 4 projetos fictícios incluídos

Para personalizar cada projeto:
- Substitua as imagens (URLs do Unsplash)
- Altere título, descrição e tecnologias
- Adicione/remova badges de tecnologia

### 5. Contato e Redes Sociais

**WhatsApp** (Linha 612):
```html
href="https://wa.me/5511999999999?text=..."
```
Substitua `5511999999999` pelo seu número com código do país.

**Redes Sociais** (Linhas 625-648):
- GitHub: Linha 627
- LinkedIn: Linha 632
- Fiverr: Linha 637
- Email: Linha 642

**Footer** (Linhas 685-692):
- Email: Linha 686
- WhatsApp: Linha 690
- Localização: Linha 694

### 6. Imagens

#### Opção 1: Usar suas próprias imagens

1. Adicione suas imagens na pasta `assets/images/`
2. No HTML, substitua as URLs do Unsplash:

```html
<!-- Antes -->
<img src="https://images.unsplash.com/photo-...">

<!-- Depois -->
<img src="assets/images/sua-imagem.jpg">
```

#### Opção 2: Continuar usando Unsplash (grátis)

As imagens atuais são do Unsplash e funcionam perfeitamente. Você pode:
- Manter como está
- Buscar outras imagens em [unsplash.com](https://unsplash.com)
- Copiar o link da imagem e colar no atributo `src`

## Deploy na Vercel

### Método 1: Deploy via GitHub (Recomendado)

1. **Crie um repositório no GitHub**
   - Acesse [github.com](https://github.com) e faça login
   - Clique em "New repository"
   - Nomeie como `portfolio-website`
   - Mantenha como "Public"

2. **Faça upload dos arquivos**
   ```bash
   cd /c/Users/sixbr/portfolio-website
   git init
   git add .
   git commit -m "Initial commit: Portfolio website"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/portfolio-website.git
   git push -u origin main
   ```

3. **Deploy na Vercel**
   - Acesse [vercel.com](https://vercel.com)
   - Clique em "Sign Up" e faça login com GitHub
   - Clique em "Add New Project"
   - Selecione seu repositório `portfolio-website`
   - Clique em "Deploy"
   - Aguarde 1-2 minutos

4. **Pronto!** Sua URL será: `https://portfolio-website.vercel.app`

### Método 2: Deploy Direto (Upload Manual)

1. **Acesse a Vercel**
   - Vá para [vercel.com](https://vercel.com)
   - Faça login (pode usar GitHub, GitLab ou email)

2. **Upload do projeto**
   - Clique em "Add New Project"
   - Selecione "Upload Files"
   - Arraste a pasta `portfolio-website` ou selecione os arquivos
   - Clique em "Deploy"

3. **Seu site estará online!**

### Configurar Domínio Personalizado (Opcional)

Se você comprou um domínio (ex: `seusite.com.br`):

1. No painel da Vercel, clique no seu projeto
2. Vá em "Settings" > "Domains"
3. Adicione seu domínio
4. Siga as instruções para configurar os DNS

## Como Testar Localmente

### Opção 1: Abrir diretamente no navegador

1. Navegue até a pasta do projeto
2. Dê duplo clique no arquivo `index.html`
3. O site abrirá no seu navegador padrão

### Opção 2: Usar um servidor local (recomendado)

**Com Python (se tiver instalado):**
```bash
cd /c/Users/sixbr/portfolio-website
python -m http.server 8000
```
Acesse: `http://localhost:8000`

**Com Node.js e npx:**
```bash
cd /c/Users/sixbr/portfolio-website
npx serve
```

**Com VS Code:**
- Instale a extensão "Live Server"
- Clique com botão direito no `index.html`
- Selecione "Open with Live Server"

## Otimizações de SEO

### Meta Tags Básicas (Já Incluídas)
- Title tag
- Description
- Keywords
- Open Graph tags

### Melhorias Adicionais

1. **Google Analytics** (opcional):
   - Crie uma conta em [analytics.google.com](https://analytics.google.com)
   - Adicione o código de tracking antes do `</head>`

2. **Favicon**:
   - Crie um favicon em [favicon.io](https://favicon.io)
   - Adicione antes do `</head>`:
   ```html
   <link rel="icon" type="image/png" href="favicon.png">
   ```

3. **Sitemap.xml**:
   - Crie um arquivo `sitemap.xml` na raiz:
   ```xml
   <?xml version="1.0" encoding="UTF-8"?>
   <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
     <url>
       <loc>https://seusite.vercel.app/</loc>
       <lastmod>2025-01-01</lastmod>
       <priority>1.0</priority>
     </url>
   </urlset>
   ```

## Integração com Formulário de Contato

O formulário atual apenas simula o envio. Para receber emails reais:

### Opção 1: EmailJS (Grátis)

1. Crie conta em [emailjs.com](https://www.emailjs.com)
2. Configure um serviço de email
3. Adicione o código EmailJS antes do `</body>`:

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
<script type="text/javascript">
  (function(){
    emailjs.init("SUA_PUBLIC_KEY");
  })();
</script>
```

4. Modifique a função de submit do formulário

### Opção 2: FormSubmit (Grátis, Mais Simples)

1. No formulário (linha 547), altere para:
```html
<form action="https://formsubmit.co/seuemail@exemplo.com" method="POST">
  <!-- campos do formulário -->
</form>
```

2. Substitua `seuemail@exemplo.com` pelo seu email

## Performance

O site já está otimizado para performance:

- Tailwind CSS via CDN (carregamento rápido)
- Fontes com `display=swap` (evita FOIT)
- Imagens via Unsplash CDN (otimizadas automaticamente)
- JavaScript vanilla (sem bibliotecas pesadas)
- Lazy loading de imagens

### Teste de Performance

Após o deploy, teste em:
- [PageSpeed Insights](https://pagespeed.web.dev)
- [GTmetrix](https://gtmetrix.com)

Você deve obter scores 90+ em Performance!

## Suporte

Se tiver dúvidas ou problemas:

1. Verifique se todos os links foram personalizados
2. Teste o site localmente antes do deploy
3. Confira os logs de erro no console do navegador (F12)

## Próximos Passos

Após o deploy:

1. ✅ Teste o site em diferentes dispositivos
2. ✅ Configure Google Analytics (opcional)
3. ✅ Adicione seu domínio personalizado (se tiver)
4. ✅ Compartilhe o link no seu perfil Fiverr
5. ✅ Atualize projetos reais conforme os desenvolve
6. ✅ Adicione mais seções se necessário (blog, depoimentos, etc)

## Licença

Este projeto é de uso livre. Personalize e use como quiser!

---

**Desenvolvido com 💙 e muito código**

Boa sorte com seu portfólio e seus projetos na Fiverr! 🚀
