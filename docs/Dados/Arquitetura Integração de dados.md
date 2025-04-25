As empresas são obrigadas a utilizar múltiplos sistemas distintos em suas operações diárias. Os sistemas operacionais nas áreas de CRM, ERP, Recursos Humanos e Marketing são especializados e desenvolvidos para funções específicas.

Embora esses produtos sejam muito bons para a finalidade pretendida, usá-los como um repositório central de dados para todos os dados de uma organização para fins operacionais, análises avançadas e operações de IA/ML pode ser desafiador.

A integração serve ao propósito de reunir e consolidar dados de diversas fontes e consolida-los para criar insights ou análises com uma perspectiva mais ampla .

Os conceitos de **integração de dados** não sejam novos, o cenário dinâmico de dados em formato e tipo, aliado a um cenário tecnológico em rápida transformação, justifica uma revisão das diversas arquiteturas de integração disponíveis e suas tecnologias associadas.

Qualquer necessidade empresarial que exija dados de vários sistemas distintos exigirá algum tipo de recurso de integração de dados, sejam eles: Integração de dados SaaS, Referência/Sincronização de Dados Mestres, Padronizar metadados dentro de pipelines de integração e consolidar dados de várias funções empresariais para obter insights e relatórios ricos.

![](../img/data_integration_reference_architecture.png)

A arquitetura de integração de dados concentra-se em **determinar a abordagem correta para a consolidação de dados** com base no formato dos dados, no caso de uso e nos métodos e tecnologias existentes.

A arquitetura possui oito componentes: 

- [ ] Fontes de dados baseadas em armazenamento ;
- [ ] Extração, transformação e carregamento (ETL);
- [ ] Extração, carga e transformação (ELT);
- [ ] Serviço de cluster/corretor de eventos;
- [ ] Processamento de fluxo;
- [ ] Gateway de API;
- [ ] Armazenamentos de dados de destino;
- [ ] Visualização de dados;
- [ ] Gerenciamento de metadados.

A arquitetura de referência mostra 4(quatro) maneiras pelas quais os dados de origem baseados em armazenamento podem ser acessados:

- [ ] **Acesso direto a dados**:  Uma conexão direta a uma fonte de dados para ler dados.
- [ ] **Acesso ao log de transações**: Acesso a um log de transações disponível para ler dados, metadados ou comandos.
- [ ] **Acesso ao formato de tabela aberta**: Uma camada de abstração que permite a extração de dados.
- [ ] **Chamadas de API** : Emita comandos por meio de APIs fornecidas por SaaS para acessar dados armazenados em sistemas de CRM/RH/ERP.

A arquitetura de referência também descreve dois fluxos de dados que descrevem para onde os dados são enviados após a integração.

- [ ] **Conexão direta com armazenamentos de dados de destino**:  Conexão direta com armazenamentos de dados de destino para gravar/armazenar dados integrados.
- [ ] **Virtualização de dados em armazenamentos de dados de destino** : Por meio da virtualização de dados, os dados de armazenamentos de dados de destino são mesclados virtualmente para testes, modelagem ou visualização de dados.

A arquitetura é composta por 8 (oito) categorias de componentes , com 3 (três) componentes principais focados nos métodos de integração:

- [ ] **Fontes de dados baseadas em armazenamento**: Localização dos dados que serão integrados.
- [ ] **ETL/ELT/ETLT**: Software e serviços que compõem a funcionalidade principal de integração, como transformação, união, limpeza, validação e orquestração de pipelines de dados.
- [ ] **Cluster/serviço de agente de eventos** : O principal componente de middleware orientado a eventos responsável por receber eventos publicados de fontes e entregá-los (por meio de tópicos e/ou configuração de assinatura) aos coletores de eventos inscritos.
- [ ] **Processamento de fluxo** : O mecanismo que lê mensagens de corretores de eventos e executa transformações e integrações.
- [ ] **Gateway de API** : APIs fornecidas por aplicativos SaaS para acessar seus dados e processos. Aplicativos SaaS normalmente oferecem esse método em vez de permitir extrações diretas de suas estruturas de dados internas.
- [ ] **Armazenamentos de dados de destino**: Local onde os dados pós-integrados serão armazenados.
- [ ] **Gerenciamento de metadados** : Captura de metadados para fins de linhagem ou dicionário de dados em pipelines de dados.
- [ ] **Virtualização de dados** : Um método de integração virtual que pode virtualizar dados de várias fontes de dados integradas.

### Armazenamento

Fontes de dados baseadas em armazenamento :

- [ ] **Sistemas de gerenciamento de banco de dados relacional**:  Bancos de dados relacionais tradicionais que armazenam dados em tabelas com índices.
- [ ] **Data lake** — Um data lake atua como um armazenamento central para todos os tipos de formatos de dados. O armazenamento normalmente ocorre em um sistema de arquivos, o que facilita a ingestão. No entanto, as extrações podem ser desafiadoras. Formatos de tabela abertos fornecem uma camada abstrata que pode ser aproveitada para acessar data lakes.
- [ ] **Lakehouse** — Lakehouses são uma arquitetura relativamente recente que incorpora os conceitos de um data lake e de um data warehouse. Um lakehouse combina os recursos de um data lake com os pontos fortes de um data warehouse, que pode armazenar dados em formatos relacionais e permitir consultas.
- [ ] **Aplicações SaaS** — São sistemas empresariais específicos, voltados para uma função empresarial. Normalmente, o sistema possui seu próprio método de armazenamento, com regras e processos proprietários que atuam sobre os dados.
- [ ] **BDs não relacionais** — São repositórios de dados que armazenam e organizam dados em um formato não relacional. Incluem pares chave-valor, documentos e BDs vetoriais.
