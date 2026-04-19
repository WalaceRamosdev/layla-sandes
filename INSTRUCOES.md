# Plano de Implementação: Website Layla Sandes

O site foi desenvolvido com foco em **autoridade, acolhimento e conversão**, utilizando as tecnologias mais modernas do ecossistema Astro.

## 🏗️ Estrutura do Projeto

O site segue uma arquitetura **MPA (Multi-Page Application)** para máximo desempenho de SEO.

- **Frontend**: Astro 5.0 + TailwindCSS 4.0 (Vite)
- **Animações**: GSAP + ScrollTrigger (Efeitos de revelação suaves)
- **SEO**: Schema.org Psychologist, Meta tags dinâmicas e Blogs com foco local.

### 🎨 Design System
- **Cores**: Tons de bege (#FDFBF7), Areia (#D4B7A1) e detalhes em Grafite Suave.
- **Tipografia**: 
  - *Outfit*: Usada para títulos, transmitindo sofisticação e leveza.
  - *Inter*: Usada para textos corridos, garantindo legibilidade máxima.

## 📄 Páginas Criadas

1.  **Home (`index.astro`)**: Hero persuasivo, pain points dos pacientes, prova social e CTAs estratégicos.
2.  **Sobre (`sobre.astro`)**: Narrativa humanizada e autoridade profissional.
3.  **Serviços (`servicos/index.astro` e `servicos/[slug].astro`)**: Páginas individuais para Ansiedade, Depressão, Relacionamentos e Autoconhecimento.
4.  **Blog (`blog/index.astro` e `blog/[slug].astro`)**: Estrutura pronta para conteúdo (Markdown) focada em SEO local.
5.  **Contato (`contato.astro`)**: Formulário otimizado e acesso direto ao WhatsApp.

## 🚀 Próximos Passos (Ação do Usuário)

Como o ambiente de execução de comandos está com restrições, siga estes passos para colocar o site no ar:

### 1. Instalação de Dependências
Abra o terminal na pasta do projeto e execute:
```bash
npm install
```

### 2. Organização de Imagens
Mova as imagens geradas para a pasta `public/images/`:
- Renomeie a imagem da psicóloga para `hero.png`.
- Adicione ícones ou fotos profissionais para os posts do blog em `public/images/`.

### 3. Personalização Final
No código, procure por termos entre colchetes e substitua pelos dados reais da Dra. Layla:
- `[Sua Cidade]` -> Ex: Salvador, São Paulo, etc.
- `[CRP]` -> Registro Profissional.
- `[WhatsApp]` -> Link Real do WhatsApp na `Layout.astro` e `Footer.astro`.

### 4. Execução Local
Para visualizar o site em desenvolvimento:
```bash
npm run dev
```

## 📈 Estratégia de SEO
- **H1 e H2**: Otimizados com variações de "Psicóloga em [Cidade]".
- **Schema Markup**: Incluído no `Layout.astro` para que o Google reconheça como um negócio local de psicologia.
- **Slug**: URLs amigáveis como `/servicos/ansiedade-em-cidade`.
