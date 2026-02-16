# 📘 RichFAQ: Gerador de FAQ Universal & SEO

> **Versão 1.0** | *Otimizado para UX e Google Rich Snippets*

O **RichFAQ** é uma ferramenta *client-side* (SPA) robusta desenvolvida para transformar textos simples em componentes HTML complexos, interativos e semanticamente otimizados para SEO. Ela resolve dois problemas críticos de criadores de conteúdo e desenvolvedores: a criação de interfaces elegantes (Accordion/Expandable) e a geração automática de Dados Estruturados (JSON-LD) para o Google.

---

## 📋 Índice

1. [Visão Geral](#-visão-geral)
2. [Como Usar](#-como-usar-guia-rápido)
3. [Guia de Estilização (CSS & IA)](#-guia-de-estilização-com-ia)
4. [Arquitetura Técnica](#-arquitetura-técnica)
5. [Instalação e Download](#-instalação-e-download)
6. [Roadmap e Futuro](#-roadmap)

---

## 🚀 Visão Geral

O RichFAQ funciona diretamente no navegador, sem necessidade de banco de dados ou backend. Ele oferece:
- **HTML Semântico:** Uso de tags `<details>` e `<summary>`.
- **SEO Automático:** Gera o script JSON-LD `FAQPage` para Rich Snippets.
- **Markdown Support:** Formatação rica (negrito, links, listas) dentro das respostas.
- **Persistência Local:** Salva seus temas e configurações no navegador.

---

## 📖 Como Usar (Guia Rápido)

### Passo 1: Escolha o Layout
No topo da ferramenta, selecione o modo desejado:
* **🔘 Accordion / FAQ:** Cria uma lista de perguntas expansíveis. Gera HTML + JSON-LD.
* **🔘 Texto Expansível / SEO:** Cria um bloco de texto com botão "Ler Mais" usando *CSS Checkbox Hack* (funciona sem JS).

### Passo 2: Insira o Conteúdo
O sistema utiliza detecção inteligente de texto:
1.  **Título:** Defina o H2 da seção.
2.  **Editor:**
    * Para criar uma **Pergunta**, termine a linha com um ponto de interrogação (**?**).
    * As linhas seguintes são automaticamente detectadas como **Resposta**.
    * Use Markdown à vontade (ex: `**negrito**`, `[link](url)`).

> **Dica:** Deixe uma linha em branco entre cada par de pergunta/resposta para organizar melhor.

### Passo 3: Personalize e Exporte
* Use o **Editor CSS** para ajustar cores e fontes (veja a seção de Estilização abaixo).
* Clique em **"Salvar"** para guardar seu tema no LocalStorage.
* Clique em **"Gerar Código FAQ"** para obter o HTML e o JSON-LD prontos para colar no seu site.

---

## 🎨 Guia de Estilização com IA

Você não precisa ser um expert em CSS. O RichFAQ expõe as classes para que você possa pedir ajuda a uma IA (como Gemini ou ChatGPT).

### Classes Disponíveis

#### Modo Accordion
| Classe | Descrição |
| :--- | :--- |
| `.faq-container` | Wrapper principal. |
| `.faq-title` | Título H2 da seção. |
| `.faq-item` | Item individual (`<details>`). |
| `.faq-question` | Texto clicável da pergunta (`<summary>`). |
| `.faq-answer` | Conteúdo da resposta. |

#### Modo Texto SEO
| Classe | Descrição |
| :--- | :--- |
| `.seo-text-container` | Wrapper principal. |
| `.seo-content` | Área do texto (com limite de altura). |
| `.seo-btn-label` | Botão "Ler mais/menos". |

### 🤖 Prompt para Copiar e Colar na IA
Copie o texto abaixo e envie para o Gemini/ChatGPT para gerar estilos incríveis:

> "Eu tenho um código HTML gerado pelo RichFAQ que usa as seguintes classes CSS: `.faq-container`, `.faq-title`, `.faq-item`, `.faq-question`, `.faq-answer`.
> Gostaria que você gerasse um código CSS completo e responsivo para essas classes.
> **Estilo desejado:** [INSIRA AQUI: Ex: Minimalista, Dark Mode, com bordas arredondadas e cores azuis]."

---

## ⚙️ Arquitetura Técnica

O RichFAQ foi construído sob uma arquitetura monolítica para máxima portabilidade:

1.  **Single Page Application (SPA):** Todo a lógica reside em um único arquivo `index.html`.
2.  **Regex Parsing:** Um algoritmo lê o texto cru e identifica padrões de perguntas (`?`) e quebras de linha para estruturar o HTML.
3.  **Local Storage:** Utiliza a API do navegador para salvar e carregar temas personalizados do usuário, garantindo privacidade (nenhum dado é enviado para a nuvem).
4.  **Performance:**
    * **Accordion:** Usa tags nativas do navegador, sem dependência de bibliotecas pesadas.
    * **Texto SEO:** Usa a técnica "Pure CSS Checkbox Hack" (`:checked ~ div`), permitindo interatividade sem JavaScript no site final.

---

## ⬇️ Instalação e Download

Para garantir que você está usando a versão mais segura e atualizada do RichFAQ, recomendamos clonar ou baixar este repositório diretamente.

### Como baixar
1.  Clique no botão verde **<> Code** acima e selecione **Download ZIP**.
2.  Extraia a pasta no seu computador.
3.  Abra o arquivo `index.html` no seu navegador favorito.


---

## 🔮 Roadmap

O projeto está em constante evolução. Funcionalidades planejadas para as próximas versões:

- [ ] **Biblioteca de Temas:** Estilos pré-definidos (Google Style, Clean, Dark).
- [ ] **Upload de Imagens:** Suporte nativo para imagens dentro das respostas.
- [ ] **Validador de Schema:** Verificação em tempo real de erros no JSON-LD.
- [ ] **Exportação CMS:** Botões dedicados para WordPress, Shopify e Elementor.

---

**Desenvolvido com foco em Performance e SEO.**
*Gostou da ferramenta? Deixe uma ⭐ neste repositório!*
