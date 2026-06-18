# 📄 Documentação — Site Rapeedo
**Arquivo principal:** `home.html`  
**Pasta do projeto:** `C:\Users\damar\Documents\SITE RAPEEDO\`  
**Última atualização:** Maio de 2026

---

## 📁 Estrutura de Arquivos

```
SITE RAPEEDO/
├── home.html                  ← Página principal (todo o site)
├── index.html                 ← Redireciona para home.html
├── 404.html                   ← Página de erro personalizada
├── politica-de-privacidade.html ← Política de privacidade
├── login.html                 ← Página de login
├── manifest.json              ← PWA (Progressive Web App)
├── status.json                ← Status da rede em tempo real
├── logo.png                   ← Logo padrão
├── VerticalBranca.png         ← Logo branca (usada no rodapé)
├── 1.jpg / 2.jpg / 3.jpg      ← Imagens auxiliares
├── img/
│   ├── logo-rapeedo.png       ← Logo principal (navbar e favicon)
│   ├── slide-residencial.jpg  ← Imagem do slide Residencial
│   ├── slide-gamer.jpg        ← Imagem do slide Gamer
│   ├── slide-empresarial.jpg  ← Imagem do slide Empresarial
│   ├── equipe-rapeedo.jpg     ← Foto da equipe (seção Quem Somos)
│   ├── atendimento-rapeedo.jpg ← Foto atendimento (Como Funciona)
│   └── tecnico-instalacao.jpg ← Foto técnico (Como Funciona)
└── libs/
    ├── chart.min.js           ← Biblioteca de gráficos
    └── pptxgen.bundle.js      ← Geração de apresentações
```

---

## 🎨 Identidade Visual

### Paleta de Cores (Modo Claro)
| Variável       | Cor       | Uso                        |
|---------------|-----------|----------------------------|
| `--blue`      | `#0050A4` | Cor principal da marca     |
| `--blue-dark` | `#0A2C66` | Cabeçalhos, hero, rodapé   |
| `--orange`    | `#EC6C04` | Destaque, CTA, plano featured |
| `--bg-light`  | `#DCE6F8` | Fundos leves, ícones        |
| `--neutral`   | `#F2F2F2` | Fundo geral da página       |
| `--text`      | `#1a1d23` | Texto principal             |
| `--muted`     | `#6b7280` | Texto secundário            |
| `--white`     | `#ffffff` | Branco padrão               |

### Paleta de Cores (Modo Escuro)
| Variável       | Cor       |
|---------------|-----------|
| `--blue`      | `#4d9fff` |
| `--blue-dark` | `#1a3a7a` |
| `--orange`    | `#ff8c3a` |
| `--neutral`   | `#111827` |
| `--text`      | `#f1f5f9` |
| `--white`     | `#0f172a` |

### Tipografia
- **Fonte:** Inter (Google Fonts) — pesos 400, 500, 600, 700, 800, 900
- **Scroll suave:** `html { scroll-behavior: smooth; }`

---

## 🗂️ Seções da Página

### 1. Barra de Anúncio (`#annBar`)
- Faixa azul no topo com oferta de instalação grátis
- Link direto para WhatsApp
- Botão `✕` para fechar

### 2. Navbar (`.navbar`)
- Logo à esquerda, links à direita
- Menu dropdown **"Soluções"** (desktop: hover | mobile: link direto para `#solucoes`)
- Links: Planos · Cobertura · Quem somos · Ajuda
- Botões: Status da Rede · Modo Escuro · Busca · Área do Cliente
- **Mobile:** hamburger menu com menu fullscreen

### 3. Carrossel Hero (`#carousel`)
4 slides automáticos (5 segundos cada):
- **Residencial** — foto `slide-residencial.jpg`
- **Gamer** — foto `slide-gamer.jpg`
- **Empresarial** — foto `slide-empresarial.jpg`
- **Smart** — foto `slide-smart` (gradiente azul)

Controles: setas `◀ ▶`, dots de navegação, barra de progresso animada.

### 4. Barra de Estatísticas (`#stats-bar`)
Números animados (contagem ao entrar na tela):
- **27+** Cidades atendidas
- **25k+** Clientes conectados
- **99%** Uptime de rede
- **15 anos** No Vale do Jequitinhonha

### 5. Soluções (`#solucoes`)
4 cards em grade:
- **Residencial** → redireciona para aba Residencial nos planos
- **Gamer** → redireciona para aba Gamer nos planos
- **Empresarial** → redireciona para aba Empresarial
- **Smart** → redireciona para aba Smart

### 6. Como Funciona (`#como-funciona`)
3 passos com fotos reais:
1. Escolha seu plano (foto atendimento)
2. Agendamos a instalação (foto técnico)
3. Conectado! (foto residencial)

### 7. Planos (`#planos`)
4 abas com swipe horizontal no mobile:

**Residencial:**
| Plano         | Velocidade | Preço   | Streaming         |
|---------------|-----------|---------|-------------------|
| Combo Alegria | 500 Mb    | R$99,90 | —                 |
| Combo Vigor ⭐ | 800 Mb    | R$119,90| Paramount+        |
| Combo Supremo | 1 Giga    | R$149,90| Paramount+ + Max  |

**Gamer:** 500/800 Mbps — IP público, ExitLag incluso  
**Empresarial:** SLA contratual, IP fixo, suporte local  
**Smart:** Câmeras, gravação em nuvem, app Olli  

Todos os botões abrem WhatsApp com mensagem pré-preenchida.

### 8. Cobertura (`#cobertura`)
- Mapa interativo Leaflet.js com marcadores
- Lista de 27+ cidades atendidas (MG e BA)
- Campo de busca para filtrar cidades
- Tooltip com nome da cidade ao clicar no marcador

### 9. Tabela Comparativa
Comparação entre planos com ícones ✓/✗  
Scroll horizontal no mobile com indicador "deslize →"

### 10. Autoridade / Diferenciais
Números e selos de confiança em grade 2×4

### 11. Por que a Rapeedo? (`#por-que`)
6 cards com diferenciais:
- Fibra própria · NOC 24h · Equipe local · IP público · SLA · Dados em tempo real

### 12. Depoimentos (`#depoimentos`)
3 avaliações de clientes reais  
**Mobile:** swipe horizontal, cards compactos, altura uniforme

### 13. Suporte (`#suporte`) — "Estamos aqui para você"
3 cards de contato:
- WhatsApp (33) 3038-1955
- 0800 276 0176 (gratuito)
- Central online / NOC 24h

**Mobile:** swipe horizontal, igual aos depoimentos

### 14. Quem Somos (`#quem-somos`)
- Texto institucional: história desde 2005, fundação em 2008 em Medina-MG
- Foto da equipe
- Números: 2005, 2008, 27 cidades, 25k+ clientes
- Princípios da empresa

### 15. FAQ (Perguntas Frequentes)
6 perguntas em accordion (`<details>`/`<summary>`):
- Área de cobertura
- Prazos de instalação
- Diferença fibra óptica vs. cabo
- Franquia de dados
- Suporte técnico
- E outras

### 16. CTA Final
Chamada para ação com botões:
- "Ver planos" → `#planos`
- "Falar no WhatsApp" → WhatsApp
- "Testar velocidade" → teste.rapeedo.com.br

### 17. Rodapé (`.footer`)
- **Logo branca** (`VerticalBranca.png`) centralizada no mobile
- Tagline: "Somos Rapeedo. Velocidade que vai além da conexão."
- Ícones sociais: Instagram · Facebook · WhatsApp
- **Navegue** e **Contato** lado a lado (mobile)
- Informações: endereço, telefone, e-mail
- CNPJ 10.403.034/0001-80 · Autorizado ANATEL · Desde 2008

---

## 🔧 Funcionalidades JavaScript

### Carrossel
```js
carouselGo(index)   // Vai para slide específico
carouselMove(dir)   // Move +1 ou -1
resetTimer()        // Reinicia o temporizador de 5s
```

### Planos
```js
setTab(name)  // 'residencial' | 'gamer' | 'empresarial' | 'smart'
```

### Busca
```js
openSearch()   // Abre overlay de busca
closeSearch()  // Fecha overlay
```

### Menu Mobile
```js
toggleMenu()        // Abre/fecha menu hamburger
toggleDropdown()    // Toggle submenu Soluções (desktop)
closeDropdown()     // Fecha submenu
```

### Contato / Painel
```js
openContactPanel()   // Abre painel lateral de contato
closeContactPanel()  // Fecha painel
```

### Quiz "Qual é o Meu Plano?"
```js
openQuizModal()    // Abre modal do quiz
closeQuizModal()   // Fecha modal
```

### LGPD / Cookies
```js
lgpdAccept()  // Aceita cookies → remove banner
lgpdClose()   // Fecha banner sem aceitar
```
> Banner aparece automaticamente após 1,8 segundos (modo teste).  
> Para produção: substituir `setTimeout` por verificação de cookie `localStorage`.

### Status da Rede
- Carrega `status.json` a cada 60 segundos
- Atualiza badge colorido na navbar (verde/amarelo/vermelho)
```js
loadNetworkStatus()  // Busca status.json e atualiza UI
openStatusModal()    // Abre modal de status detalhado
closeStatusModal()   // Fecha modal
```

### Contador Animado
```js
animateCounters()  // Anima os números da stats bar ao entrar na tela
```

### Mapa de Cobertura
```js
filterCities(term)  // Filtra lista de cidades
```
Utiliza **Leaflet.js** com tiles OpenStreetMap.

### Scroll Reveal
Elementos com classe `.reveal` animam ao entrar na viewport via `IntersectionObserver`.

### Modo Escuro
```js
toggleDark()  // Alterna body.dark — salva em localStorage
```

### Voltar ao Topo
Botão fixo no canto inferior esquerdo — aparece após scroll de 300px.

### WhatsApp Flutuante
Botão fixo verde no canto inferior direito.  
**Mobile:** posicionado acima da barra de navegação inferior.

---

## 📱 Comportamento Mobile (`max-width: 768px`)

| Elemento           | Comportamento Mobile                         |
|--------------------|----------------------------------------------|
| Navbar             | Hamburger menu fullscreen                    |
| Soluções (nav)     | Link direto para `#solucoes` (sem dropdown)  |
| Carrossel          | Altura 420px, texto adaptado                 |
| Cards de Soluções  | Grade 2×2                                    |
| Planos             | Swipe horizontal (scroll-snap)               |
| Mapa               | 280px de altura                              |
| Tabela comparativa | Scroll horizontal                            |
| Depoimentos        | Swipe horizontal, cards compactos uniformes  |
| Suporte            | Swipe horizontal, cards compactos uniformes  |
| Side tabs          | Barra de navegação fixada no rodapé (62px)   |
| CTA Final          | Botões empilhados verticalmente              |
| Rodapé             | Logo centralizada, Navegue+Contato lado a lado|
| WhatsApp float     | `bottom: 74px` (acima da nav bar)            |
| Cookie bar         | `bottom: 62px` (acima da nav bar)            |

---

## 📲 Barra de Navegação Mobile (Side Tabs)

3 botões fixos no rodapé da tela:
| Botão               | Cor     | Ação                        |
|--------------------|---------|-----------------------------|
| Fale Conosco       | Azul    | Abre painel de contato      |
| Teste de Velocidade| Laranja | Abre teste.rapeedo.com.br   |
| Qual é o Meu Plano?| Roxo    | Abre modal quiz             |

---

## 🌐 Integrações Externas

| Serviço             | URL / Detalhe                              |
|--------------------|--------------------------------------------|
| Google Fonts        | Inter (400–900)                            |
| Leaflet.js          | Mapa interativo de cobertura               |
| WhatsApp            | `wa.me/553330381955`                       |
| Área do Cliente     | `sistema.rapeedo.com.br`                   |
| Teste de Velocidade | `teste.rapeedo.com.br`                     |
| Google Analytics 4  | ID: `G-XXXXXXXXXX` ← **substituir pelo ID real** |
| VLibras             | Acessibilidade em Libras (Gov. Federal)    |

---

## 🔍 SEO / Meta Tags

```html
<title>Rapeedo — Internet Fibra Óptica no Vale do Jequitinhonha</title>
<meta name="description" content="...planos de 500Mb a 1Giga...">
<meta property="og:title" ...>
<meta property="og:image" content="img/slide-residencial.jpg">
<meta property="og:url" content="https://rapeedo.com.br">
<meta name="twitter:card" content="summary_large_image">
```

**Schema.org (JSON-LD):**
```json
{
  "@type": "InternetCafe",
  "name": "Rapeedo",
  "telephone": "+55-33-3038-1955",
  "address": { "streetAddress": "Rua Francisco Neiva, 87", "addressLocality": "Medina", "addressRegion": "MG" }
}
```

---

## ⚠️ Pendências / Coisas para Configurar antes de Publicar

1. **Google Analytics** — substituir `G-XXXXXXXXXX` pelo Measurement ID real
2. **Cookie LGPD** — trocar o `setTimeout` por verificação de `localStorage` para não mostrar sempre
3. **status.json** — manter atualizado com status real da rede
4. **og:url** — confirmar que está `https://rapeedo.com.br`
5. **og:image** — garantir que a imagem seja acessível publicamente

---

## 📞 Contatos no Site

| Canal         | Detalhe                          |
|--------------|----------------------------------|
| WhatsApp     | (33) 3038-1955                   |
| 0800         | 0800 276 0176 (gratuito)         |
| E-mail       | contato@rapeedo.com.br           |
| Endereço     | Rua Francisco Neiva, 87 — Medina, MG |
| CNPJ         | 10.403.034/0001-80               |
| Instagram    | @rapeedointernet                 |
| Facebook     | /rapeedo                         |

---

*Documentação gerada em Maio de 2026.*
