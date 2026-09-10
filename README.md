# PDF Editor Studio 📄✨

O **PDF Editor Studio** é um aplicativo web leve, moderno e **100% cliente-side** (executado totalmente no navegador) projetado para a visualização, marcação e inserção precisa de imagens/carimbos (PNG/JPEG) em documentos PDF de múltiplas páginas.

Ele foi especialmente otimizado para rodar diretamente via arquivo local (`file:///`), sem a necessidade de servidores locais (Node.js, Python, Apache) ou dependências de background.

---

## 🚀 Funcionalidades

- **Carregamento Local Seguro:** Funciona nativamente ao abrir o arquivo `.html` diretamente no navegador com dois cliques (compatível com protocolo `file:///` sem restrições de CORS).
- **Suporte Multi-Páginas:** Renderização fluida de documentos PDF com várias páginas.
- **Quadro Flutuante de Posicionamento:**
  - Moldura flutuante com suporte a arrastar e soltar (*drag & drop*) e redimensionamento livre.
  - Acompanha a rolagem da tela (*viewport fixed*) em qualquer extensão do documento.
- **Inserção de Imagens (PNG/JPEG):**
  - Converte e projeta a imagem diretamente na página e posição selecionadas pelo quadro.
  - Mantém o aspecto transparente de arquivos PNG.
- **Edição Interativa:** Redimensionamento, rotação e reposicionamento livre da imagem inserida através da biblioteca interativa `Fabric.js`.
- **Exportação Fiel:** Gera e faz o download do novo arquivo PDF mantendo a escala, qualidade e proporção originais das inserções.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 & CSS3:** Interface moderna em Dark Mode, com CSS Variables e posicionamento avançado.
- **JavaScript (ES6+):** Manipulação de eventos, lógica de coordenadas e leitura de dados assíncronos.
- **[PDF.js](https://mozilla.github.io/pdf.js/):** Renderização e visualização de arquivos PDF em Elementos Canvas.
- **[Fabric.js](http://fabricjs.com/):** Manipulação interativa de objetos e vetores na camada sobreposta ao PDF.
- **[PDF-Lib](https://pdf-lib.js.org/):** Leitura, modificação e compilação final do arquivo PDF binário.

---

## 📦 Como Usar

### Pré-requisitos
Apenas um navegador web moderno (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari ou Opera). **Não é necessário instalar bibliotecas, Python ou servidores locais.**

### Passo a Passo

1. **Baixar o Projeto:**
   Baixe e salve o arquivo `pdfeditorV5.html` em uma pasta no seu computador.

2. **Abrir o Editor:**
   Dê **dois cliques** no arquivo `pdfeditorV5.html` para abri-lo diretamente no seu navegador.

3. **Carregar um PDF:**
   - Arraste um arquivo `.pdf` para a área indicada na tela **OU**
   - Clique na barra superior em **"Carregar PDF"** e selecione o documento.

4. **Posicionar Imagem/Carimbo:**
   - Clique no botão **"+ Posicionar Quadro"** na barra superior.
   - Arraste e redimensione o quadro tracejado sobre o local da página onde deseja inserir a imagem.
   - Clique no botão **"carregar PNG"** no centro do quadro flutuante e selecione sua imagem.

5. **Ajustar a Imagem:**
   - Com a imagem inserida na página, use os manipuladores nos cantos para ajustar a escala, rotacionar ou mover a posição final.

6. **Salvar o Documento:**
   - Clique em **"Salvar PDF"** no canto superior direito para baixar o documento alterado (`documento_assinado.pdf`).

---

## 🔒 Privacidade e Segurança

Todas as operações de processamento, leitura e geração do PDF são realizadas **exclusivamente na memória do navegador do seu computador**. Nenhum documento ou imagem é enviado para servidores externos.