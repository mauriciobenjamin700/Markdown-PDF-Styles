# Tutorial: Configurando o Arquivo settings.json do VS Code para Geração de PDF com Estilo Externo

Neste tutorial, vamos aprender como configurar o arquivo `settings.json` do Visual Studio Code para usar a extensão Markdown PDF e aplicar um estilo externo a partir de um arquivo CSS hospedado online.

## Passo 1: Instalação da Extensão Markdown PDF

Antes de começar, certifique-se de ter a extensão Markdown PDF instalada no Visual Studio Code. Você pode encontrar a extensão na loja de extensões do VS Code ou instalar diretamente pelo link: [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf)

## Passo 2: Criação do Arquivo settings.json

1. Abra o Visual Studio Code.
2. Pressione `Ctrl + Shift + P` (Windows/Linux) ou `Cmd + Shift + P` (Mac) para abrir a paleta de comandos.
3. Digite "Preferences: Open Settings (JSON)" e pressione Enter para abrir o arquivo `settings.json`.

## Passo 3: Configuração do Arquivo settings.json

Agora, vamos adicionar as configurações necessárias ao arquivo `settings.json`.

```json
{
    "markdown-pdf.styles": [
        "https://caminho/para/seu/arquivo/estilo.css"
    ],
    "markdown-pdf.includeDefaultStyles": false,
    "markdown-pdf.margin.top": "2cm",
    "markdown-pdf.margin.bottom": "2cm",
    "markdown-pdf.margin.left": "2cm",
    "markdown-pdf.margin.right": "2cm",
    "markdown-pdf.scale": 1,
    "markdown-pdf.width": "210mm",
    "markdown-pdf.height": "297mm"
}
```

Certifique-se de substituir `"https://caminho/para/seu/arquivo/estilo.css"` pelo URL real do seu arquivo CSS hospedado online.

## Passo 4: Gerando o PDF

Após salvar as configurações no arquivo `settings.json`, você pode gerar o PDF do seu documento Markdown seguindo estes passos:

1. Abra o arquivo Markdown que deseja converter para PDF.
2. Pressione `Ctrl + Shift + P` (Windows/Linux) ou `Cmd + Shift + P` (Mac) para abrir a paleta de comandos.
3. Digite `Markdown PDF: Export (pdf)` e pressione Enter para iniciar a conversão.
4. O PDF será gerado e salvo automaticamente no mesmo diretório do arquivo Markdown, a menos que você tenha especificado um diretório de saída diferente nas configurações.

Parabéns! Agora você configurou com sucesso o arquivo `settings.json` do VS Code para chamar um arquivo de estilo externo e gerar PDFs formatados de seus documentos Markdown.
