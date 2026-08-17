# 📄 Dynamic CV Generator & PDF Exporter

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white) ![Tech](https://img.shields.io/badge/Tech-Stack-007ACC?style=for-the-badge) ![Library](https://img.shields.io/badge/Library-Dependencies-6C63FF?style=for-the-badge)

Um gerador de currículos interativo feito para facilitar a criação, formatação e exportação de dados profissionais. O usuário preenche os blocos de informações através de abas expansíveis (*accordions*) e exporta o documento final perfeitamente estruturado em formato **PDF** com um único clique.

---

## ✨ Funcionalidades Principais

- **➕ Campos Dinâmicos:** Adicione quantos cursos profissionais e experiências profissionais desejar através de botões de inserção dinâmica via manipulação do DOM.
- **🗂️ Interface com Accordion:** Organização modular dos formulários em painéis expansíveis e colapsáveis nativos para melhorar a experiência visual.
- **🖨️ Exportação em PDF:** Integração assíncrona com a biblioteca externa `html2pdf.js`, convertendo elementos estruturados em arquivos PDF prontos para impressão.
- **🔄 Gerenciamento Dinâmico de Telas:** Troca de estados do contêiner principal para alternar de forma limpa entre o formulário de captação de dados e a visualização prévia do currículo.

---

## 🛠️ Tecnologias Utilizadas

O projeto utiliza puramente recursos web nativos integrados com uma biblioteca de conversão:

- **HTML5:** Estrutura base de inputs, formulários semânticos, seletores e injeção assíncrona de templates.
- **CSS3:** Estilização de formulários, controle de transições visuais das abas abertas/fechadas (`.active`, `.panel`) e formatação focada na folha de impressão.
- **JavaScript Vanilla (ES6):**
  - Manipulação profunda do DOM através de `insertAdjacentHTML` e seletores dinâmicos.
  - Varredura algorítmica incremental (`while`) para agrupar dinamicamente arrays de objetos de múltiplos cursos e experiências enviados via `FormData`.
- **html2pdf.js (via CDN):** Engine responsável por transformar trechos específicos do DOM em arquivos PDF estruturados.

---

## 📂 Estrutura do Repositório

Para implantar e rodar o projeto diretamente no GitHub Pages sem erros, certifique-se de manter os arquivos nesta disposição na raiz do seu repositório:

```text
├── index.html        # Estrutura HTML principal e importação do html2pdf.js
├── style.css         # Estilização das caixas de input e lógica visual dos painéis
└── script.js        # Motor JS, lógica dos botões de adição e conversão do PDF
```

---

## 🎮 Como Rodar Localmente

1. Clone o repositório em seu ambiente local:
   ```bash
   git clone https://github.com/leo-gomes-dev/gerador_de_curriculo_pdf.git
   ```
2. Entre na pasta raiz do projeto.
3. Abra o arquivo `index.html` diretamente em seu navegador web.
4. Comece a preencher o formulário, teste o botão **"Adicionar curso +"** e submeta os dados para gerar o seu documento.



