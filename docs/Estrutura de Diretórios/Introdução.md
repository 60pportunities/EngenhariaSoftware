No contexto de gerenciamento de ativos digitais, podemos definir como a inclusão de todos os arquivos e ativos digitais organizados hierarquicamente dentro de um estrutura de diretório.

  Enfatizamos alguns componentes principais e convenções :

| Termo                           | Descrição                                                                                                                                       |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Hierarquia                      | O resultado é uma hierarquia em forma de árvore que organiza ativos com base em seus relacionamentos e categorias.                              |
| Categorias                      | A estrutura de pasta representa uma categoria lógica.                                                                                           |
| Consistência                    | Convenção de nomenclatura irão garantir que seja fácil para os usuários navegar e localizar ativos em toda a estrutura de arquivos rapidamente. |
| Controle de acesso              | Considere controle de acesso e permissões mais restritos para pastas que contêm ativos sensíveis.                                               |
| Controle de versão              | Se for essencial, considere em coloca-lo em SCM.                                                                                                |
| Estrutura de diretórios         | Diretórios são frequentemente usados como a unidade de organização primária.                                                                    |
| Estrutura de arquivo de pasta   | Pastas são comumente usadas em interfaces gráficas de usuário.                                                                                  |
| Diretório raiz                  | O diretório raiz fica no topo da árvore.                                                                                                        |
| Diretório pai                   | Exceto pela raiz, cada diretório tem um pai. O diretório pai contém o diretório atual.                                                          |
| Subdiretórios/diretórios filhos | Abaixo do diretório raiz e dos diretórios pais estão os subdiretórios (também chamados de diretórios filhos).                                   |

### Simples, Clara, Flexivel e Escalável

| NÍVEL           | NÍVEL        | NÍVEL      | NÍVEL           | NÍVEL        | NÍVEL    | NÍVEL     | NÍVEL       |
| --------------- | ------------ | ---------- | --------------- | ------------ | -------- | --------- | ----------- |
| PARTICULAR      |              |            |                 | PROFISSIONAL |          |           |             |
|                 | FAMILIA      |            |                 |              | CLIENTES |           |             |
|                 |              | FOTOS      |                 |              |          | CONVERSAS |             |
|                 |              |            | LOCAL           |              |          |           | REUNIAO     |
|                 |              | DOCUMENTOS |                 |              |          | PROJETOS  |             |
|                 |              |            | CERTIFICADOS    |              |          |           | PROJETO_001 |
|                 |              | FINANCAS   |                 |              |          |           | PROJEOT_002 |
|                 |              |            | IMPOSTO_RENDA   |              |          |           |             |
|                 |              |            | CONTAS_PUBLICAS |              |          |           |             |
|                 |              |            | AQUISICOES      |              |          |           |             |
|                 |              |            | MERCADO_LIVRE   |              |          |           |             |
|                 |              |            | ALIEXPRESS      |              |          |           |             |
|                 |              |            | SHOPPE          |              |          |           |             |
| DESENVOLVIMENTO |              |            |                 |              |          |           |             |
|                 | LINGUAGEM    |            |                 |              |          |           |             |
|                 |              | PL_SQL     |                 |              |          |           |             |
|                 |              | GO_LANG    |                 |              |          |           |             |
|                 |              | BASH       |                 |              |          |           |             |
|                 | CONFIGURACAO |            |                 |              |          |           |             |
|                 |              | GITCONFIG  |                 |              |          |           |             |
|                 |              | SENHAS     |                 |              |          |           |             |
|                 |              | DRIVERS    |                 |              |          |           |             |
|                 |              |            |                 |              |          |           |             |
|                 | REPOSITORIOS |            |                 |              |          |           |             |
|                 | MKDOCS       |            |                 |              |          |           |             |
|                 |              | PROJETO-A  |                 |              |          |           |             |
## Estruturas Base
Ao longo da atividade da Tecnologia da Informação, inúmeros foram as explicações para a elaboração de uma estutura BASE de caminhos ou diretórios.
No Linux, a organização segue o **Filesystem Hierarchy Standard (FHS)**, que define padrões para hierarquia de pastas.
No Windows, a organização é mais flexível, mas há convenções comuns, que serão exemplificadas.
Os repositórios Git seguem convenções para organização de código e colaboração, mas apenas o diretório .git, possui uma estrutura. Repositórios remotos (GitHub, GitLab, SVN) ou de dados (como bancos de dados) seguem algum tipo de padrão em função do fornecedor ou produto.
Estruturas do maven, possui vários archetypes e cada um com a sua estrutura.
#### **Por que Padronizar?**

- [ ] **Consistência**: Facilita a navegação e colaboração em equipe.
- [ ] **Versionamento Eficiente**: Evita conflitos no Git.
- [ ] **Portabilidade**: Projetos funcionam em diferentes sistemas operacionais.
- [ ] **Manutenibilidade**: Encontrar arquivos rapidamente em cenários de debug ou escalabilidade.
Essas estruturas são **sugestões baseadas em boas práticas**, mas podem ser adaptadas conforme as necessidades do projeto ou convenções da equipe. Consulte a [[Estruturas Base]].

## Nomenclatura de Arquivos
Aqui estão as melhores práticas, a meu ver,  para nomear arquivos no **Windows** e **Linux**, considerando as particularidades de cada sistema:

|                          |                                                                                                 |
| ------------------------ | ----------------------------------------------------------------------------------------------- |
| **Caracteres proibidos** | \ / : * ? " < > \| `/` e `\0` (                                                                 |
| **Nomes reservados**     | como `CON`, `PRN`, `AUX`, `NUL`, `COM1`, `LPT1` etc.                                            |
| **Extensões**            | Mantenha extensões consistentes (ex: `.docx`, `.jpg`) para associar corretamente aos programas. |
| **Evite espaços**        | Substitua por hífens (`-`) ou underscores (`_`). Ex: `meu-arquivo.txt`.                         |
| **Compatibilidade**      | Prefira nomes em **ASCII** (evite acentos se o sistema for compartilhado).                      |
| **Formato de data**      | Use `YYYY-MM-DD` para ordenação automática.                                                     |
| **Letras minúsculas**    | Padronize para evitar conflitos (especialmente em sistemas mistos).                             |
| **Versões e números**    | Versionamento Semantico                                                                         |
| **Comprimento máximo**   | Não ultrapasse de **255 bytes**                                                                 |
Exemplo:

- [ ] relatorio_vendas_YYYY-MM-DD_SEMVER.pdf
- [ ] XXXXX_folha_de_ponto_YYYY-MM-DD_SEMVER.pdf
