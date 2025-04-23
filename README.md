# Desafio BLOG :: Entendimento da aula das tags apreendidas e de outros tópicos

***Basicamente o instrutor explica de forma básica e coerente os pontos abaixo: ***

## *Índice*

* [Ferramentas utilizadas](#Ferramentas)
* [Usando o Inspetor de Elementos](#Usando)
* [Estrutura básica do HTML](#Estrutura)
* [Falando sobre Tags](#Falando)
* [Atributos básicos](#Atributos)
* [Executando uma página HTML](#Executando)
* [Textos](#Textos)
* [Listas ordenadas e não ordenadas](#Listas)
* [Links](#Links)
* [Contato Instrutor](#Contato)
* [Bibliografia e Sites Recomendados para HTML](#Bibliografia)

## Ferramentas utilizadas

[Voltar](#Índice)

### Instalação e Preparação do VS Code para HTML

#### Passo 1: Baixar o VS Code

1.  Abra o seu navegador de internet (Chrome, Firefox, Edge, etc.).
2.  Acesse o site oficial do Visual Studio Code: [https://code.visualstudio.com/](https://code.visualstudio.com/)
3.  O site deve detectar automaticamente o seu sistema operacional e exibir o botão de download correto.
4.  Clique no botão para baixar a versão estável.
5.  Aguarde o download do arquivo de instalação ser concluído.

#### Passo 2: Instalar o VS Code

##### Windows:

* Localize o arquivo `.exe` baixado (geralmente em "Downloads").
* Dê um duplo clique no arquivo para iniciar a instalação.
* Leia e aceite o contrato de licença.
* Clique em "Avançar" nas telas seguintes, mantendo as opções padrão.
* Marque a opção "Adicionar ao PATH".
* Clique em "Instalar" e aguarde a conclusão.
* Clique em "Concluir" para abrir o VS Code.

##### macOS:

* Localize o arquivo `.dmg` baixado (geralmente em "Downloads").
* Dê um duplo clique no arquivo `.dmg`.
* Arraste o ícone do VS Code para a pasta "Applications".
* Abra a pasta "Applications" e clique duas vezes no ícone do Visual Studio Code para iniciá-lo.

##### Linux:

* Escolha o arquivo adequado para sua distribuição (`.deb`, `.rpm`, `.tar.gz`).
* **Para `.deb` (exemplo Ubuntu):** Abra o terminal, navegue até a pasta e execute: `sudo dpkg -i <nome_do_arquivo>.deb`, seguido de `sudo apt-get update && sudo apt-get install -f`.
* **Para `.rpm` (exemplo Fedora):** Abra o terminal, navegue até a pasta e execute: `sudo rpm -i <nome_do_arquivo>.rpm`.
* **Para `.tar.gz`: **Descompacte e execute o arquivo `code` dentro da pasta. Considere criar um link simbólico.

#### Passo 3: Preparar o VS Code para HTML

1.  **Abrir uma pasta de projeto (recomendado):**
    * Crie uma pasta no seu computador (ex: "meu_projeto_web").
    * Abra o VS Code.
    * Vá em "Arquivo" (File) > "Abrir Pasta..." (Open Folder...).
    * Selecione a pasta e clique em "Selecionar Pasta" (Select Folder).
2.  **Criar um arquivo HTML:**
    * Na barra lateral esquerda, clique no ícone de "Novo Arquivo".
    * Digite o nome do arquivo com a extensão `.html` (ex: `index.html`) e pressione Enter.
3.  **Escrever seu código HTML:**
    * Comece a digitar a estrutura HTML básica (experimente digitar `!` e pressionar `Tab`).

    ```html
    <!DOCTYPE html>
    <html lang="pt-br">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Minha Página HTML</title>
    </head>

    <body>
        <h1>Olá, Mundo!</h1>
        <p>Este é meu primeiro código HTML no VS Code.</p>
    </body>

    </html>
    ```

4.  **Salvar o arquivo:**
    * Vá em "Arquivo" (File) > "Salvar" (Save) ou pressione `Ctrl + S` (Windows/Linux) / `Cmd + S` (macOS).
5.  **Visualizar no navegador:**
    * Abra a pasta onde você salvou o arquivo `.html`.
    * Dê um duplo clique no arquivo para abri-lo no navegador.

#### Dicas Extras para HTML no VS Code:

* **Emmet:** Já integrado, facilita a escrita de HTML e CSS com abreviações (ex: digite `li*3` e pressione `Tab`).
* **Extensões (opcional, mas útil):**
    * **HTML CSS Support:** Autocompletar para classes e IDs CSS.
    * **Auto Rename Tag:** Renomeia tags de abertura e fechamento simultaneamente.

## Usando o Inspetor de Elementos

[Voltar](#Índice)

O **Inspetor de Elementos** é uma ferramenta essencial, integrada diretamente nos navegadores web modernos como Google Chrome, Mozilla Firefox, Microsoft Edge e Apple Safari. Ele serve como uma janela para o "código de bastidores" de qualquer página web que você visita. Através dele, é possível examinar e até mesmo modificar temporariamente a estrutura **HTML** (que define o conteúdo e a organização dos elementos na página) e o **CSS** (que controla a apresentação visual desses elementos, como cores, fontes e layout).

### Para que serve o Inspetor de Elementos?

* **Entender a estrutura HTML:** Ele permite visualizar a hierarquia de elementos HTML, mostrando como as diferentes tags estão aninhadas e organizadas para formar a página. Você pode expandir e recolher nós para explorar a estrutura em detalhes.
* **Analisar o CSS aplicado:** Para cada elemento HTML selecionado, o Inspetor de Elementos exibe as regras de CSS que estão afetando sua aparência. Isso inclui estilos definidos em arquivos CSS externos, dentro da tag `<style>` no próprio HTML e estilos inline (no atributo `style`).
* **Modificação em tempo real:** Uma das funcionalidades mais poderosas é a capacidade de editar o HTML e o CSS diretamente na interface do Inspetor. As alterações são refletidas instantaneamente na visualização da página no seu navegador. É importante lembrar que essas modificações são apenas locais e temporárias; ao recarregar a página, o conteúdo original é restaurado.
* **Depuração de Layout e Estilo:** Se um elemento não está aparecendo ou se comportando como esperado visualmente, o Inspetor de Elementos ajuda a identificar quais regras de CSS estão causando o problema. Você pode desativar ou modificar estilos para testar diferentes soluções.
* **Aprendizado e Inspeção de Outros Sites:** Ao navegar por diferentes sites, você pode usar o Inspetor de Elementos para aprender como eles são construídos e estilizados. Isso pode ser uma ótima fonte de inspiração e conhecimento.
* **Análise de Desempenho (em algumas abas):** Ferramentas relacionadas no mesmo conjunto (como a aba "Rede" ou "Performance") permitem analisar o tempo de carregamento de recursos e outros aspectos do desempenho da página.

### Como acessar o Inspetor de Elementos?

Existem várias maneiras de abrir o Inspetor de Elementos:

1.  **Clique com o botão direito do mouse:** A maneira mais comum é clicar com o botão direito sobre o elemento específico que você deseja examinar (ou em qualquer lugar da página) e selecionar a opção **"Inspecionar"** ou **"Inspecionar Elemento"** no menu de contexto que aparece.
2.  **Atalhos de teclado:** A maioria dos navegadores oferece atalhos de teclado para abrir o Inspetor de Elementos:
    * **Google Chrome, Microsoft Edge, Brave:** Pressione a tecla `F12` ou a combinação de teclas `Ctrl + Shift + I` (no Windows e Linux) ou `Cmd + Option + I` (no macOS).
    * **Mozilla Firefox:** Pressione a tecla `F12` ou a combinação de teclas `Ctrl + Shift + I` (no Windows e Linux) ou `Cmd + Option + I` (no macOS).
    * **Apple Safari:** Primeiro, você precisa ativar o menu "Desenvolvedor" nas preferências do Safari. Vá em "Safari" > "Preferências..." > "Avançado" e marque a caixa "Mostrar menu Desenvolvedor na barra de menus". Depois disso, você pode clicar com o botão direito e selecionar "Inspecionar Elemento" ou usar o atalho `Option + Cmd + I`.

### O que você vê ao abrir o Inspetor de Elementos?

Ao abrir o Inspetor, geralmente você verá a janela do navegador dividida em duas seções principais:

* **Aba "Elementos" (ou "Elements"):** Esta aba mostra a estrutura HTML da página como uma árvore hierárquica de elementos. Você pode navegar por essa árvore, expandindo e recolhendo os nós para ver a relação entre as tags. Ao selecionar um elemento nesta aba, ele é destacado visualmente na página web.
* **Aba "Estilos" (ou "Styles"):** Localizada geralmente ao lado ou abaixo da aba "Elementos", esta seção exibe as regras de CSS que estão sendo aplicadas ao elemento atualmente selecionado na aba "Elementos". Você pode ver as propriedades CSS, seus valores, e em qual arquivo ou tag de estilo cada regra está definida.

### Em resumo:

O **Inspetor de Elementos** é uma ferramenta indispensável para qualquer pessoa que trabalha com desenvolvimento web. Ele oferece uma visão profunda de como as páginas são construídas e estilizadas, permitindo inspeção, análise e experimentação em tempo real.

## Estrutura básica do HTML

[Voltar](#Índice)

### O que é a estrutura básica do HTML?

Todo documento HTML válido segue uma estrutura fundamental. Essa estrutura garante que o navegador entenda como interpretar e exibir o conteúdo da página corretamente. Os elementos essenciais são:

* `<!DOCTYPE html>`: A declaração `DOCTYPE` informa ao navegador que este é um documento HTML5. Deve ser a primeira linha do seu código HTML.
* `<html>`: A tag `<html>` é o elemento raiz de toda página HTML. Todos os outros elementos (exceto a declaração `DOCTYPE`) devem estar dentro desta tag. O atributo `lang` dentro da tag `<html>` especifica o idioma principal do documento (por exemplo, `lang="pt-br"` para português do Brasil).
* `<head>`: A tag `<head>` contém metadados sobre o documento HTML, que não são exibidos diretamente na página. Informações como o título da página (que aparece na aba do navegador), a codificação de caracteres, informações para SEO e links para arquivos CSS são colocados dentro da tag `<head>`.
* `<body>`: A tag `<body>` contém todo o conteúdo visível da página HTML, como textos, imagens, links, vídeos e outros elementos interativos.

### Exemplo de estrutura básica:

```html
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>
</head>

<body>
    <h1>Meu Primeiro Título</h1>
    <p>Este é um parágrafo.</p>
</body>

</html>
