# 📄 Currículo Profissional - Carla Gomes Cunha

Um currículo profissional moderno, responsivo e acessível desenvolvido com HTML5 e CSS3. Este projeto demonstra as melhores práticas de desenvolvimento web front-end.

![Preview do Currículo](https://img.shields.io/badge/Status-Concluído-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

## 🎯 Sobre o Projeto

Este currículo foi desenvolvido para a professora Carla Gomes Cunha, apresentando suas qualificações profissionais de forma clara e profissional. O design é totalmente responsivo e segue as melhores práticas de acessibilidade web.

### ✨ Características Principais

- 🎨 **Design Moderno**: Interface limpa e profissional
- 📱 **Totalmente Responsivo**: Adapta-se a qualquer dispositivo
- ♿ **Acessível**: Segue as diretrizes WCAG 2.1
- 🔍 **SEO Otimizado**: Meta tags para melhor indexação
- 🖨️ **Impressão Otimizada**: Layout específico para impressão
- ⚡ **Performance**: Código otimizado e eficiente

## 🚀 Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e acessível
- **CSS3**: Estilos modernos com variáveis CSS
- **Responsive Design**: Media queries para diferentes dispositivos
- **Acessibilidade**: ARIA labels e roles

## 📁 Estrutura do Projeto

```
curriculo/
├── index.html          # Estrutura HTML principal
├── styles.css          # Estilos CSS
├── 3x4.png            # Foto de perfil
└── README.md          # Documentação do projeto
```

## 🎨 Estrutura HTML

### Seções Principais

```html
<header class="cabecalho">          <!-- Cabeçalho com nome -->
<main class="conteiner">            <!-- Container principal -->
  <aside class="esquerda">          <!-- Coluna lateral -->
    <section class="contato">       <!-- Informações de contato -->
    <section class="habilidades">   <!-- Habilidades -->
    <section class="idiomas">       <!-- Níveis de idiomas -->
    <section class="cursos">        <!-- Cursos realizados -->
  </aside>
  <div class="direita">             <!-- Coluna principal -->
    <section class="resumo">        <!-- Resumo profissional -->
    <section class="experiencia">   <!-- Experiência profissional -->
    <section class="formacao">      <!-- Formação acadêmica -->
  </div>
</main>
<footer class="rodape">             <!-- Rodapé -->
```

## 🎯 Classes CSS Principais

### Layout

- `.cabecalho` - Cabeçalho da página
- `.conteiner` - Container principal com flexbox
- `.esquerda` - Coluna lateral (30% da largura)
- `.direita` - Coluna principal (70% da largura)
- `.rodape` - Rodapé da página

### Seções de Conteúdo

- `.contato` - Informações de contato
- `.habilidades` - Lista de habilidades
- `.idiomas` - Níveis de proficiência em idiomas
- `.cursos` - Cursos e certificações
- `.resumo` - Resumo profissional
- `.experiencia` - Experiência de trabalho
- `.formacao` - Formação acadêmica

### Elementos Específicos

- `.foto-perfil` - Container da foto de perfil
- `.barra-idioma` - Barras de progresso para idiomas
- `.trabalho` - Experiências profissionais individuais
- `.diploma` - Formação acadêmica
- `.atual` - Indicador de emprego atual

## 🎨 Variáveis CSS

O projeto utiliza variáveis CSS para facilitar a manutenção:

```css
:root {
  --primary-color: #003366; /* Cor principal */
  --secondary-color: #f4f4f4; /* Cor de fundo */
  --text-color: #333; /* Cor do texto */
  --light-gray: #e6e6e6; /* Cinza claro */
  --border-color: #999; /* Cor das bordas */
  --shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Sombra */
  --border-radius: 5px; /* Raio das bordas */
  --spacing-sm: 5px; /* Espaçamento pequeno */
  --spacing-md: 10px; /* Espaçamento médio */
  --spacing-lg: 20px; /* Espaçamento grande */
  --font-size-small: 14px; /* Fonte pequena */
  --font-size-medium: 16px; /* Fonte média */
  --font-size-large: 18px; /* Fonte grande */
}
```

## 📱 Responsividade

### Breakpoints

- **Desktop**: Layout de duas colunas (30% + 70%)
- **Tablet (≤768px)**: Layout em coluna única
- **Mobile (≤480px)**: Otimizado para telas pequenas

### Media Queries

```css
@media (max-width: 768px) {
  .conteiner {
    flex-direction: column;
  }
  .esquerda,
  .direita {
    width: 100%;
  }
}

@media (max-width: 480px) {
  .cabecalho h1 {
    font-size: 1.25rem;
  }
}
```

## ♿ Acessibilidade

### Implementações

- ✅ Atributos `role` apropriados
- ✅ `aria-label` para elementos interativos
- ✅ `aria-valuenow` para barras de progresso
- ✅ Estados de foco visíveis
- ✅ Contraste de cores adequado (WCAG AA)
- ✅ Tamanhos de fonte legíveis
- ✅ Estrutura semântica HTML5

### Exemplo de Implementação

```html
<div
  class="barra-idioma"
  role="progressbar"
  aria-valuenow="90"
  aria-valuemin="0"
  aria-valuemax="100"
  aria-label="Nível de inglês: 90%"
>
  <span class="nivel-90"></span>
</div>
```

## 🔍 SEO e Metadados

### Meta Tags Implementadas

```html
<meta
  name="description"
  content="Currículo de Carla Gomes Cunha - Professora de Português"
/>
<meta
  name="keywords"
  content="professora, português, educação, ensino fundamental"
/>
<meta name="author" content="Carla Gomes Cunha" />
```

### Open Graph (Redes Sociais)

```html
<meta property="og:title" content="Currículo - Carla Gomes Cunha" />
<meta property="og:description" content="Professora de Português" />
<meta property="og:image" content="3x4.png" />
```

## 🖨️ Otimização para Impressão

```css
@media print {
  .cabecalho {
    background-color: var(--primary-color) !important;
    -webkit-print-color-adjust: exact;
  }
  .conteiner {
    box-shadow: none;
    margin: 0;
  }
}
```

## 🚀 Como Usar

### 1. Clone o Repositório

```bash
git clone [url-do-repositorio]
cd curriculo
```

### 2. Personalize o Conteúdo

- Edite `index.html` para alterar informações pessoais
- Modifique `styles.css` para ajustar cores e estilos
- Substitua `3x4.png` pela sua foto de perfil

### 3. Ajuste as Cores (Opcional)

```css
:root {
  --primary-color: #sua-cor-principal;
  --secondary-color: #sua-cor-secundaria;
}
```

### 4. Visualize

Abra `index.html` em qualquer navegador moderno.

## 🎯 Funcionalidades

### Links Interativos

- **Telefone**: `tel:+5599999999999`
- **Email**: `mailto:carla.cunha@email.com.br`
- **LinkedIn**: Abre em nova aba

### Animações

- Hover effects nos links
- Transições suaves nas barras de progresso
- Animação na foto de perfil

### Barras de Progresso

- Visualização do nível de idiomas
- Animações CSS
- Acessibilidade completa

## 📊 Performance

### Otimizações Implementadas

- ✅ CSS minificado (em produção)
- ✅ Imagens otimizadas
- ✅ Lazy loading para imagens
- ✅ Código limpo e eficiente

### Métricas Esperadas

- **Lighthouse Performance**: 95+
- **Lighthouse Accessibility**: 100
- **Lighthouse SEO**: 100
- **Lighthouse Best Practices**: 100

## 🛠️ Desenvolvimento

### Pré-requisitos

- Navegador moderno (Chrome, Firefox, Safari, Edge)
- Editor de código (VS Code, Sublime Text, etc.)

### Estrutura de Desenvolvimento

1. **HTML**: Estrutura semântica
2. **CSS**: Estilos e responsividade
3. **Testes**: Validação de acessibilidade
4. **Otimização**: Performance e SEO

## 🧪 Testes

### Validação HTML

```bash
# Use o validador W3C
https://validator.w3.org/
```

### Validação CSS

```bash
# Use o validador W3C CSS
https://jigsaw.w3.org/css-validator/
```

### Teste de Acessibilidade

- Use ferramentas como axe DevTools
- Teste com leitores de tela
- Verifique contraste de cores

## 📈 Melhorias Futuras

### Funcionalidades Planejadas

- [ ] Modo escuro/claro
- [ ] Download em PDF
- [ ] Versão em inglês
- [ ] Seção de projetos
- [ ] Filtros por categoria
- [ ] Animações mais elaboradas

### Otimizações Técnicas

- [ ] CSS Grid para layout mais avançado
- [ ] JavaScript para interatividade
- [ ] PWA (Progressive Web App)
- [ ] Integração com CMS

## 🤝 Contribuição

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 👤 Autor

**Carla Gomes Cunha**

- LinkedIn: [linkedin.com/in/carla-gomes-cunha](https://linkedin.com/in/carla-gomes-cunha)
- Email: carla.cunha@email.com.br

## 🙏 Agradecimentos

- Inspiração em designs modernos de currículo
- Comunidade de desenvolvedores web
- Ferramentas de validação e teste

---

⭐ **Se este projeto foi útil, considere dar uma estrela!**

**Desenvolvido com ❤️ seguindo as melhores práticas de desenvolvimento web moderno.**
#   c u r r i c u l o 
 
 
