A arquitetura de referência fornece um modelo padronizado, orientando arquitetos e equipes de engenharia a aderir às melhores práticas e padrões comprovados, garantindo que a aplicação seja otimizada para escalabilidade, resiliência e eficiência no ambiente nativo da nuvem.

Ela se concentra na definição de uma arquitetura altamente disponível, escalável e resiliente que se adapta aos casos de uso mais comuns que a Gartner vê seus clientes utilizando.

A arquitetura de aplicativos nativos da nuvem é comumente aplicada aos seguintes casos de uso :
- [ ] Back-ends escaláveis ​​para aplicativos web e mobile — A arquitetura de aplicativos nativos em nuvem se alinha à natureza dinâmica dos aplicativos web e mobile modernos. Ao adotar contêineres, computação sem servidor e arquitetura orientada a eventos, os desenvolvedores podem construir back-ends que escalam, se adaptam às demandas em constante mudança e oferecem experiências consistentes e confiáveis ​​ao usuário, independentemente do uso.
- [ ] Microsserviços — Os microsserviços são projetados para serem fracamente acoplados, implantáveis ​​e escaláveis ​​de forma independente. Essas características os tornam um bom exemplo para a arquitetura de aplicativos nativos da nuvem.
- [ ] Arquitetura de aplicativos centrada em API — A arquitetura de aplicativos nativos em nuvem pode ajudar organizações a expor recursos de negócios aos seus clientes por meio de APIs bem definidas.

![](../img/reference_architecture_for_cloud_native_applications.png)
#### A arquitetura de referência é composta por 10 componentes principais

- [ ] **Automação de construção e lançamento** — Um processo automatizado, na plataforma do provedor de nuvem ou no local, que facilita a criação, o teste, a digitalização, o empacotamento e a implantação de artefatos e/ou imagens de contêiner.
- [ ] **Proteção contra ameaças da Web e controle de acesso**: Componentes necessários para permitir que o aplicativo da Web se comunique com o back-end.
- [ ] **Monitoramento e observabilidade de serviços de aplicativos**: Capacidade de instrumentar serviços e aplicativos que podem ajudar a investigar problemas que podem não ter sido previstos.
- [ ] **Rede resiliente em nuvem**: Um conjunto de serviços em nuvem que ajudam a implementar alta disponibilidade, tolerância a falhas e confiabilidade em uma infraestrutura de rede em nuvem.
- [ ] **Gateway de API**:  Componente que fornece um ponto de entrada controlado para os consumidores dos serviços. O gateway inclui serviços de segurança e identidade de API e aplica políticas como limites de taxa e limitação.
- [ ] **Gerenciamento de estado do servidor**:  Um componente opcional que deve ser implementado quando for necessário manter o controle do estado atual do usuário e/ou aplicativo no servidor.
- [ ] **Serviços Compostos** : Um componente opcional que deve ser implementado quando uma camada intermediária é necessária entre o cliente e os serviços de back-end. Este componente pode agregar dados, interagir com o serviço de gerenciamento de estado e realizar a transformação de dados antes que eles sejam retornados ao front-end.
- [ ] **Cluster/Serviço do Event Broker** : O principal componente de middleware orientado a eventos responsável por receber eventos publicados de fontes e roteá-los (por meio de tópicos e/ou configuração de assinatura) para coletores de eventos inscritos.
- [ ] **Serviços de aplicação** : Um conjunto de serviços que implementam a lógica de negócios principal de um aplicativo, acesso a dados e outras operações comerciais.
- [ ] **Application Data Services**: Componente responsável por armazenar, recuperar e manipular dados para o aplicativo.
