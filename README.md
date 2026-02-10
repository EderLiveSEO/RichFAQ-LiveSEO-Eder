# Gerador de FAQ Universal

Este projeto é uma ferramenta desenvolvida para facilitar a criação de **Perguntas Frequentes (FAQs)** com estilo de acordeão (dropdown), otimizado para SEO e com visual profissional e personalizável.

## 🎯 Finalidade
O objetivo principal é permitir que qualquer pessoa crie seções de FAQ de alta qualidade para sites, garantindo:
1.  **Visual Integrado**: O estilo padrão já é moderno, mas permite personalização completa via CSS para combinar com a identidade visual do site de destino.
2.  **SEO Friendly**: Gera automaticamente os **Dados Estruturados (JSON-LD)** necessários para que o Google entenda e destaque as perguntas nos resultados de busca.
3.  **Facilidade de Uso**: Basta colar o texto, e a ferramenta identifica automaticamente perguntas e respostas.

## 🚀 Funcionalidades Principais

*   **Detecção Automática de Perguntas**: O sistema identifica linhas terminadas em `?` como perguntas e o texto seguinte como resposta.
*   **Estilo Acordeão (Accordion)**: As perguntas funcionam como dropdowns, expandindo ao clique para mostrar a resposta.
*   **Modo Noturno (Dark Mode)**: Interface de administração com tema escuro para conforto visual, salvando a preferência do usuário.
*   **Sistema de Salvamento de Estilos**: Permite salvar configurações de CSS personalizadas (ex: "Tema Azul", "Tema Minimalista") no navegador para uso recorrente.
*   **Preview em Tempo Real**: Visualize como a FAQ ficará antes de copiar o código.
*   **Geração de Código Limpo**: Entrega HTML sem frameworks pesados e JSON-LD pronto para uso.

## 🛠️ Como Usar

1.  **Título**: Preencha o título da seção de FAQ (ex: "Dúvidas Frequentes").
2.  **Conteúdo**: Cole suas perguntas e respostas. 
    *   *Dica*: Deixe uma linha em branco entre cada par para organizar melhor.
3.  **Personalização (Opcional)**:
    *   Use o campo "Personalizar CSS" para alterar cores, fontes ou espaçamentos.
    *   Salve seu estilo para usar novamente depois com o botão "Salvar CSS".
4.  **Gerar**: Clique em "Gerar Código FAQ".
5.  **Copiar**:
    *   Copie o **HTML** e cole na área de conteúdo do seu site.
    *   Copie o **JSON-LD** e cole no `<head>` ou rodapé do seu site para melhorar o SEO.

## 💻 Tecnologias
- HTML5
- CSS3 (Variáveis CSS, Flexbox, Grid)
- JavaScript (Vanilla)

---
*Desenvolvido pela equipe LiveSEO.*
