# Pérola Noivas — Landing Page Institucional & Curadoria de Alta-Costura

## 1. Identificação Acadêmica

* **Instituição de Ensino:** Senac
* **Curso:** Técnico em Desenvolvimento de Sistemas
* **Disciplina:** Projeto Integrador
* **Orientador:** Profº Hudson Neves
* **Integrante:** Geovanna Rezende dos Santos ([@geovan-na](https://github.com/geovan-na))
* **Status do Projeto:** Concluído (MVP em Produção)
* **Ambiente de Publicação:** [https://geovan-na.github.io/P-rolaNoivas/](https://geovan-na.github.io/P-rolaNoivas/)

---

## 2. Descrição

O **Pérola Noivas** é um projeto de desenvolvimento web front-end concebido para estruturar a presença digital e a conversão de clientes de um atelier tradicional de moda nupcial de Brasília (com mais de 21 anos de história). O projeto traduz a identidade de luxo, autoridade e acolhimento da marca para uma interface moderna, inspirada em arquitetura editorial sóbria, minimalista e responsiva.

---

## 3. Objetivos

### 3.1 Objetivo Geral
Desenvolver uma landing page responsiva, de alta performance e visualmente sofisticada, capaz de exibir o catálogo de grifes internacionais e direcionar potenciais noivas para agendamento de provas exclusivas.

### 3.2 Problema que o Sistema Resolve
* **Baixa conversão em canais puramente visuais (redes sociais):** Centraliza informações institucionais, localização física, diferenciais de atendimento e grifes em um único ponto confiável na web.
* **Falta de canal direto e simplificado de agendamento:** Resolve a jornada da noiva ao disponibilizar pontos de contato integrados com mensagens pré-formatadas via WhatsApp em todas as seções-chave.
* **Apresentação visual desestruturada:** Substitui publicações dispersas por uma curadoria editorial com estética de alta-costura (lookbook de marcas, serviços detalhados e história do atelier).

### 3.3 Público-Alvo
Noivas do Distrito Federal e entorno, noivos, madrinhas e assessores de casamento que buscam vestidos de noiva de alta-costura (aluguel e confecção), acessórios finos e atendimento consultivo intimista.

---

## 4. Funcionalidades

* **Hero Section Editorial:** Apresentação da proposta de valor com imagem de alta resolução em tela cheia, tipografia com serifas clássicas e chamadas claras para ação (CTA).
* **Lookbook de Curadoria Internacional:** Seção dedicada às renomadas grifes europeias atendidas pelo atelier (**Pollardi** da Ucrânia, **Rosa Clará** e **Pronovias** da Espanha), com tags de silhuetas, acabamentos e atalhos individuais de atendimento.
* **Vitrine de Serviços:** Cards informativos com os pilares de atendimento (*Aluguel de Alta-Costura*, *Acessórios Finos* e *Prova Exclusiva Privativa* com ajustes inclusos).
* **Seção Institucional ("Nossa Promessa"):** Narrativa dos mais de 21 anos de tradição, números de confiança e selo de qualidade artesanal.
* **Menu Mobile Responsivo:** Menu hambúrguer interativo com animação fluida para dispositivos móveis e fechamento automático ao navegar.
* **Header Fixo com Efeito Glassmorphism:** Barra de navegação com transparência e desfoque dinâmico (`backdrop-filter`) que acompanha a rolagem.
* **Canal Integrado de Contato:** Botões contextuais e botão flutuante persistente de WhatsApp no canto inferior direito.
* **Guia de Localização:** Endereço completo em Taguatinga Norte com link direto integrado para abertura de rotas no Google Maps.

---

## 5. Tecnologias Utilizadas

| Categoria | Tecnologia / Ferramenta | Descrição |
| :--- | :--- | :--- |
| **Linguagem de Marcação** | **HTML5** | Estruturação semântica de conteúdo, acessibilidade e SEO. |
| **Estilização** | **CSS3 Moderno** | Variáveis customizadas (Custom Properties), Flexbox, CSS Grid, Glassmorphism e Media Queries. |
| **Interatividade** | **JavaScript (ES6+)** | Lógica de alternância do menu mobile, acessibilidade ARIA e eventos de rolagem. |
| **Tipografia** | **Google Fonts** | *Source Serif 4* (títulos e autoridade editorial) e *Cabin* (leitura limpa e contemporânea). |
| **Ícones** | **Font Awesome 6** | Biblioteca vetorial para iconografia de redes, localização e navegação. |
| **Controle de Versão** | **Git & GitHub** | Versionamento e repositório remoto. |
| **CI/CD & Deploy** | **GitHub Actions & GitHub Pages** | Pipeline automatizado de compilação e publicação estática em produção. |

---

## 6. Arquitetura da Solução

O sistema foi concebido sob o modelo arquitetural de **Single Page Application (SPA) Estática / Landing Page**.

```text
[ Cliente (Navegador Web) ]
           │
           ├── Requisição HTTP / HTTPS (GitHub Pages CDN)
           │
           ▼
[ Camada de Apresentação ]
   ├── index.html (Semântica estruturada)
   ├── style.css (Design System, Tokens e Responsividade)
   ├── assets/ (Imagens otimizadas de alta resolução)
   │
   ▼
[ Integrações Externas ]
   ├── Google Fonts API (Tipografia)
   ├── Font Awesome CDN (Iconografia)
   ├── WhatsApp Click-to-Chat API (Conversão e Atendimento)
   └── Google Maps URL Scheme (Navegação geográfica)
```

---

## 7. Modelagem do Banco de Dados

> **Nota:** Por se tratar de uma *Landing Page* institucional estática com foco em desempenho, conversão e carregamento instantâneo via CDN, o projeto **não necessita de banco de dados relacional (SGBD) ou NoSQL**. As informações e catálogos são estruturados de forma declarativa e otimizada no front-end.

---

## 8. Pré-requisitos

Para executar e visualizar o projeto localmente, são necessários apenas:
* Um navegador web moderno atualizado (Google Chrome, Mozilla Firefox, Microsoft Edge ou Safari).
* Opcionalmente, um editor de código como o **Visual Studio Code** (com a extensão *Live Server* recomendada) ou o utilitário **Git** instalado.

---

## 9. Instalação

Siga os passos abaixo para clonar e configurar o projeto em sua máquina local:

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com/geovan-na/P-rolaNoivas.git
   ```

2. **Acessar a pasta do projeto:**
   ```bash
   cd P-rolaNoivas
   ```

---

## 10. Como Executar

Por ser um projeto puramente estático, você pode executá-lo de duas formas:

### Opção 1: Execução Direta no Navegador
* Dê um duplo clique no arquivo `index.html` ou abra-o arrastando para qualquer navegador.

### Opção 2: Servidor Local (Recomendado para simular produção)
Se possuir o Node.js ou Python instalado:

* **Via Node.js (npx serve):**
  ```bash
  npx serve .
  ```
* **Via Python 3:**
  ```bash
  python -m http.server 8000
  ```
Acesse no navegador: `http://localhost:8000`

---

## 11. Estrutura do Projeto

```text
P-rolaNoivas/
├── .github/
│   └── workflows/
│       └── static.yml            # Pipeline de automação e deploy no GitHub Pages
├── assets/                       # Fotografias editoriais em alta resolução
│   ├── hero.jpg                  # Imagem principal do banner
│   ├── marca_pollardi.jpg        # Lookbook da grife Pollardi
│   ├── marca_rosaclara.jpg       # Lookbook da grife Rosa Clará
│   ├── marca_pronovias.jpg       # Lookbook da grife Pronovias
│   ├── servico_aluguel.jpg       # Imagem do serviço de aluguel de vestidos
│   ├── servico_acessorios.jpg    # Imagem do serviço de acessórios finos
│   ├── servico_consultoria.jpg   # Imagem da prova privativa exclusiva
│   └── sobre.jpg                 # Imagem editorial da seção "Nossa Promessa"
├── .impeccable/                  # Registros de auditoria e métricas de qualidade de UI/UX
├── index.html                    # Estrutura HTML5 da página
├── style.css                     # Folha de estilos e Design System responsivo
└── README.md                     # Documentação técnica do projeto integrador
```

---

## 12. Exemplos de Uso

1. **Exploração do Acervo:** A usuária acessa a página, navega pelas grifes internacionais no lookbook e consulta os estilos de cada corte (rendas, mikado, sereia, cauda).
2. **Agendamento de Visita:** Ao escolher um vestido ou serviço, clica no botão "Solicitar Atendimento" ou no botão flutuante. O sistema aciona diretamente o WhatsApp com texto pré-definido para facilitar a triagem pela equipe do atelier.
3. **Consulta de Localização:** Na seção "Localização", a usuária clica em "Abrir no Google Maps" para traçar rota direta até o atelier em Taguatinga Norte.

---

## 13. API & Integrações

O sistema utiliza integrações padronizadas via protocolos web sem dependência de chaves de API pagas:

* **WhatsApp Click-to-Chat Protocol:**
  * Endpoint: `https://wa.me/?text={MENSAGEM_CODIFICADA}`
  * Utilizado para criar canais de conversão imediatos com mensagens contextuais.
* **Google Maps URI Scheme:**
  * Endpoint: `https://maps.google.com/?q={ENDERECO_URL_ENCODED}`
  * Utilizado para direcionar para a geolocalização exata da loja física.

---

## 14. Capturas de Tela

> *As capturas de tela refletem a versão em produção publicada no GitHub Pages.*

| Seção | Prévia do Design |
| :--- | :--- |
| **Hero Principal (Desktop)** | `assets/hero.jpg` — Banner em alta resolução com tipografia editorial |
| **Curadoria de Grifes** | `assets/marca_pollardi.jpg`, `assets/marca_rosaclara.jpg`, `assets/marca_pronovias.jpg` |
| **Nossos Serviços** | `assets/servico_aluguel.jpg`, `assets/servico_acessorios.jpg`, `assets/servico_consultoria.jpg` |
| **O Atelier / História** | `assets/sobre.jpg` — Bloco assimétrico com dados institucionais |

---

## 15. Equipe do Projeto

* **Geovanna Rezende dos Santos** — *Desenvolvimento Front-End, UI/UX e Documentação*
  * GitHub: [@geovan-na](https://github.com/geovan-na)
  * E-mail: `geovannarezendedossantos@gmail.com`
* **Profº Hudson Neves** — *Orientação e Supervisão Pedagógica (Senac)*

---

## 16. Melhorias Futuras

* [ ] Implementação de um catálogo/galeria interativo com filtros por silhueta (Princesa, Sereia, Evasê, Boho).
* [ ] Formulário modal de pré-agendamento com seleção de data integrada ao Google Calendar.
* [ ] Seção de depoimentos e fotos reais de noivas atendidas pelo atelier.
* [ ] Versão bilíngue (Português / Inglês) para noivas de corpos diplomáticos e casamentos no exterior.

---

## 17. Licença

Este projeto foi desenvolvido para fins educacionais no âmbito do **Projeto Integrador do Senac**.  
Todos os direitos reservados à desenvolvedora e às marcas citadas.
