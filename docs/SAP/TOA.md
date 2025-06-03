Ela conseguiu LER o material da Oracle e não implementou pois a oracle irá remover a informação.
Elaine Berbet


BBTS
TOA - Roteirização Automática
-
Hoje, o ambiente da BBTS não tem planos de rota de forma automática para a maioria das operações.
No TOA (OFS) possui várias formas de configurar o roteirizador (atribuição recorrente, sequencial, imediata, etc), mas para implementar qualquer plano é necessário que os cadastros estejam atualizados.
Premissas para a utilização do roteirizador:
- [ ] Cadastro de Habilidades de Trabalho: são relacionadas as aptidões das equipes de camo e indicam as atividades que a equipe em capacidade para atender. Elas são exigidas para cada atividade e serão calculadas automaticamente no OFS quando cada atividade for criada;
- [ ] Cadastro de Rotas (ou áreas de trabalho): As áreas que a equipe de campo irá atuar;
- [ ] Cadastro de Locais por Recurso: Utilizar o início e fim da rota dos recursos e até mesmo atribuir uma zona central de atendimento dos recursos, raio entre 4 a 5 km.
- [ ] Cadastro de Escala de trabalho por Recurso: O recurso de campo precisa estar com sua escala de trabalho sempre atualizada com folgas previstas e configuradas para os 7 dias da semana.

A seguir, temos algumas evidencias que mostram como tais cadastros necessitam de revisão.


TOA - Cadastro de Habilidade de Trabalho
No ambiente produtivo foi identificado ordens de serviço sem habilidades de trabalho. Nas imagens abaixo ilustra um exemplo: O equipamento EQPT-091148.

Com relação as habilidades de trabalho, podemos revisa-las e até otimiza-las também.
Por exemplo, atualmente temos 10 habilidades relacionadas a impressora com scanner.
Podemos reduzi-las a uma única habilidade que abranja todas as impressoras, ou alternativamente, manter uma habilidade especifica voltada apenas para impressoras com scanner.


O local por recurso permite calcular o deslocamento em 2 situações:
• Do ponto inicial até o primeiro atendimento;
• Do último atendimento até o ponto final (Base ou casa);

Com isso, o deslocamento total do recurso é registrado.
Futuramente, podemos ter o tempo de deslocamento e o tempo de atendimento por dia através de um indicador.
Os dados ficam armazenados em uma tabela chamada appt.lake_ofs.


O perfil de campo está bem intuitivo com passo a passo bem definido no preenchimento da Ordem pelo aplicativo TOA. No entanto, o perfil pode ser revisado para que as informações não fiquem duplicadas na tela.
Como sugestão, podemos :
Destacar algumas informações importantes para o técnico. Na imagem ao lado, temos a agência destacada.
• Permite configurar e ativar o uso do workflow que permite preencher os dados da ordem de serivço em etapas.



TOA - Perfil do Backoffice
Os perfis de Backoffice, tais como: Controladores e Administradores pode ser revisado os seguintes pontos:
·
Readequação de informações com indicação mais resumidas, tais como à atividade.

Utilização de na emojis podem facilitar identificação de atividades internas ao invés de adotar o nome da atividade que podem ser extensa na visão do tempo;
Renomear nomenclaturas como o filtro ad hoc para filtro personalizado no glossário, por exemplo. A nomenclatura ficará mais clara para o entendimento do usuário.

É necessário avaliar se as imagens das ordens de serviço como a assinatura fica armazenado em um servidor especifico.
O sistema tem uma API que permite extrair os dados, se necessário. Para isso, os campos precisar estar configurados Extract
no
relatório: {companyname}_activity_details.xml. daily
Não foi identificado campos de imagens como o campo "Assinatura do cliente".


Considerações Finais

Para que os cenários de rota sejam devidamente mapeados de acordo com o tipo de atividade, calendário do recurso, área de trabalho do recurso, habilidade de trabalho do recurso e filtros específicos.

Com uma solução como o OFS/TOA não é viável que os usuários atribuem manual e façam ajustes de forma manual de atividade como objetivo de criar uma sequência pré-determinada, pois isso leva tempo para execução.

Portanto, abaixo alguns itens necessários na revisão para o aperfeiçoamento do uso do sistema:

Cadastros e Parametrizações: Garantir a correta configuração das equipes de campo dos parâmetros de roteirização como habilidade de trabalho, áreas de trabalho, calendário, locais de recursos, e principalmente filtros que possam configurar corretamente o plano de rota;

Configuração dos Planos de Rota: Na configuração dos planos com um tempo de performance para o SLR durante a execução do plano visto que parte dos planos irão roteirizar muitas atividades por dia com critérios de localização similares. Além de iniciar com planos rodando 1x por dia, na madrugada ou em horário mais cedo;

Integração (Campos): Identificado alguns tipos de atendimento que não possuem campos específicos no sistema EBS e TOA, então seria importante revisar fluxos de atendimento que possuem agendamento com Guarda de Valor,

Fabricante e concessionárias. Hoje, o controlador informa tais dados em um campo do tipo texto dificultando efetuar filtros e criar regras no TOA para priorizar tais atendimentos. O ideal é que houvesse campos especificos indicando

Data do agendamento, Agendado com ? (GV, Fabricante ou Concessionaria), Nome da GV/Fabricante/Concessionária). E somente integrar tais atividades na data do agendamento evitando poluição de atividades no TOA;

Integração ( Cadastros no EBS): Rever campos e cadastros para checar o backlog de atividades com SLA no sistema, pois algumas atividades são integradas já com SLA vencido e a Unidade tem dificuldade de uma visão geral das atividades pendentes. Além de impactar os planos de rota de forma automática na implementação.

E por fim, confiar que o roteamento fez a melhor distribuição da melhor forma de acordo com a configuração feita e que a alternativa (que são usuários fazer a atribuição ou ajuste manual) não é viável tecnicamente e financeiramente para a empresa.
