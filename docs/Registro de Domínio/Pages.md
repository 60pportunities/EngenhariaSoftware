O GitHub Pages é uma funcionalidade do GitHub que permite hospedar sites estáticos diretamente de um repositório. É uma ótima maneira de mostrar portfólios, blogs ou documentação de projetos. Aqui está um passo a passo para criar e utilizar o GitHub Pages:

- [ ] Cziar um Repositório
- [ ] Acesse sua Conta: Faça login na sua conta do GitHub.
- [ ] Criar Novo Repositório:
- [ ] Clique no botão "+" no canto superior direito e selecione "New repository".
- [ ] Dê um nome ao seu repositório. Para um site pessoal, o nome deve ser no formato username.github.io, onde username é seu nome de usuário.
- [ ] Escolha se o repositório será público ou privado. Para GitHub Pages, geralmente é **público**.
- [ ] Marque a opção "Initialize this repository with a README" para criar um README inicial.
- [ ] Clique em "Create repository".
- [ ] Adicionar Conteúdo
- [ ] Adicionar Arquivos:
- [x] No seu repositório, clique em "Add file" e depois em "Create new file".
- [ ] Crie um arquivo chamado index.html. Este será o arquivo principal do seu site.
- [ ] Adicione algum conteúdo HTML básico.
- [ ] Após adicionar o conteúdo, clique em "Commit changes".
- [ ] Por exemplo:
  
```
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Meu Site</title>
</head>
<body>
<h1>Bem-vindo ao meu site!</h1>
<p>Este é um exemplo de página usando GitHub Pages.</p>
</body>
</html>
```

- [ ] Configurar o GitHub Pages
- [ ] Acessar Configurações:
- [ ] Vá para a aba "Settings" do seu repositório.
- [ ] Selecionar GitHub Pages:
- [ ] Role para baixo até a seção "GitHub Pages".
- [ ] Em "Source", selecione a branch que deseja usar (geralmente main) e clique em "Save".
- [ ] Acessar seu Site: Após alguns minutos, seu site estará disponível no endereço https://username.github.io, onde username é seu nome de usuário. Você pode acessar e visualizar seu site diretamente pelo navegador.
- [ ] Personalizando Seu Site
- [ ] Temas: Você pode usar temas prontos para personalizar a aparência do seu site. Vá para a seção "Settings" > "Pages" e escolha um tema.
- [ ] Adicionar Mais Páginas: Crie novos arquivos HTML (por exemplo, sobre.html, contato.html) e vincule-os no seu index.html para navegar entre as páginas.
- [ ] Atualizando o Conteúdo
- [ ] Para atualizar seu site, faça alterações nos arquivos no repositório e faça novos commits. O GitHub Pages automaticamente refletirá essas mudanças no site.
  
**Observação**:

- [ ] A configuração básica seria esta, porem iremos utilizar o conceito de DaC (Doc as Code);
- [ ] Todo o documento será desenvolvido em TEXTO simples utilizando o [Markdown](https://code.visualstudio.com/docs/editor/profiles#_doc-writer-profile-template). Como padrão deste material, utilizaremos o Editor VS Code da Microsoft com algumas extensões:
	- [ ] Code Spell Checker - Verificador de ortografia para código fonte.
	- [ ] Markdown Checkboxes - Adiciona o suporte a caixa de seleção para o VS Code built-in Markdown Preview.
	- [ ] Markdown Emoji - Adiciona suporte de sintaxe emoji para Markdown Preview e células Markdown de notebook.
	- [ ] Markdown Footnotes - Adiciona o suporte de sintaxe da nota ?do para o Markdown Preview.
- [ ] Markdown Preview GitHub Styling - Use o estilo GitHub no Markdown Preview.
- [ ] Markdown Preview Mermaid Support - Diagramas e fluxogramas da Mermaid.
- [ ] Markdown yaml Preamble - Renders YAML para tabelas.
- [ ] markdownlint - Markdown linting e verificação de estilo para Visual Studio Code.
- [ ] Word Count - Visualize o número de palavras em um documento de marcação na barra de status.
- [ ] Read Time - Estime quanto tempo leva para ler o seu Markdown.
- [ ] Paste Image - Copia imagem para o texto markdown.
- [ ] PlantUML - Extensão incrível se você precisar desenhar diagramas.
- [ ] C4 DSL Extension - Especificar modelos de arquitetura de software com o Structurizr DSL.