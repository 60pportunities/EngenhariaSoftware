
## **DevOps**

```mermaid
graph TD
    A[Repositório] --> B[pipeline]
    A --> C[stages]

    B --> D[azure-pipeline.yaml]

    C --> E[manifests]
    C --> F[build.yml]
    C --> G[cleanup.yml]
    C --> H[container_scan.yml]
    C --> I[dast.yml]
    C --> J[deploy.yml]
    C --> K[push.yml]
    C --> L[sast.yml]

    E --> M[deployment.yml]
    E --> N[ingress.yml]
```


## **Estimativa**

```mermaid
mindmap
  root((PRODUTO))
    Compromisso
    Meta
    Prazo
    Estimativa
```


## **Aprendizagem**

```mermaid
flowchart TD
id1(Autoaprendizagem) --> id2(Tutoriais)
id1 --> id3(Certificações)
id1 --> id4(Projetos)
```

### **Estrutura Windows**

```mermaid
graph LR
    Root["C:/"]
    Root --> ProgramFiles["Program Files"]
    Root --> ProgramFilesx86["Program Files (x86)"]
    Root --> Users["Users"]
    Root --> Windows["Windows"]
    Root --> ProgramData["ProgramData (Hidden)"]
    Root --> PerfLogs["PerfLogs"]

    Users --> UserProfile["User Profile (e.g., Alice)"]
    Users --> Public["Public"]
    Users --> Default["Default (Template)"]

    UserProfile --> Desktop["Desktop"]
    UserProfile --> Documents["Documents"]
    UserProfile --> Downloads["Downloads"]
    UserProfile --> Pictures["Pictures"]
    UserProfile --> Music["Music"]
    UserProfile --> Videos["Videos"]
    UserProfile --> AppData["AppData (Hidden)"]

    AppData --> Local["Local"]
    AppData --> LocalLow["LocalLow"]
    AppData --> Roaming["Roaming"]

    Windows --> System32["System32"]
    Windows --> Temp["Temp"]
    Windows --> WinSxS["WinSxS (Component Store)"]

    System32 --> Drivers["Drivers"]
    System32 --> Config["Config (System Settings)"]

    ProgramFiles --> CommonFiles["Common Files"]
    ProgramFiles --> ExampleApp["Example Application"]

    ProgramFilesx86 --> LegacyApp["Legacy Application (32-bit)"]

    ProgramData --> Microsoft["Microsoft"]
    ProgramData --> AppConfigs["Application Configs"]
```
### **Estrutura Linux**

```mermaid
graph LR
    Root["/ (Root)"]
    Root --> bin["/bin (Binários Essenciais)"]
    Root --> etc["/etc (Configurações do Sistema)"]
    Root --> home["/home (Diretórios de Usuários)"]
    Root --> root["/root (Home do Superusuário)"]
    Root --> var["/var (Dados Variáveis)"]
    Root --> tmp["/tmp (Arquivos Temporários)"]
    Root --> usr["/usr (Programas e Utilitários)"]
    Root --> lib["/lib (Bibliotecas do Sistema)"]
    Root --> dev["/dev (Dispositivos de Hardware)"]
    Root --> proc["/proc (Informações do Kernel/Processos)"]
    Root --> sys["/sys (Configurações do Kernel)"]
    Root --> mnt["/mnt (Pontos de Montagem Temporários)"]
    Root --> media["/media (Mídias Removíveis)"]
    Root --> opt["/opt (Software de Terceiros)"]
    Root --> boot["/boot (Arquivos de Inicialização)"]
    Root --> run["/run (Dados de Runtime)"]
    Root --> sbin["/sbin (Binários Administrativos)"]

    home --> UserProfile["usuário (ex: alice)"]
    UserProfile --> Documents["Documents (Documentos)"]
    UserProfile --> Downloads["Downloads"]
    UserProfile --> Desktop["Desktop"]
    UserProfile --> Music["Music"]
    UserProfile --> Pictures["Pictures"]
    UserProfile --> Videos["Videos"]
    UserProfile --> Hidden[".pastas_ocultas (ex: .config, .bashrc)"]

    var --> log["/var/log (Logs do Sistema)"]
    var --> lib["/var/lib (Dados de Aplicativos)"]
    var --> www["/var/www (Servidor Web)"]

    usr --> bin["/usr/bin (Binários de Usuário)"]
    usr --> lib["/usr/lib (Bibliotecas de Aplicativos)"]
    usr --> share["/usr/share (Dados Compartilhados)"]
    usr --> src["/usr/src (Código-Fonte)"]

    etc --> network["/etc/network (Configuração de Rede)"]
    etc --> apt["/etc/apt (Repositórios APT)"]
    etc --> ssh["/etc/ssh (Configuração SSH)"]
```

## **Estrutura Git**

```mermaid
graph TD
 A01[fa:fa-home /home/user] --> C[fa:fa-folder-open git]
 C --> C01[fa:fa-folder-open core] & C02[fa:fa-folder-open hooks] &  C03[fa:fa-folder-open mensagem] & C04[fa:fa-file .gitconfig_azure] & C05[fa:fa-file .gitconfig_github]

C01 --> C0101[fa:fa-file .gitignore]

C02 --> C0201[fa:fa-file pre-commit] & C0202[fa:fa-file ....] & C0203[fa:fa-file pre-commit]

C03 --> C0301[fa:fa-file .commitmessage]
```

## **Estrutura Oracle**

```mermaid
  graph TD
  A00[fa:fa-home /home/user] --> B[fa:fa-folder-open oracle]
  B --> B01[fa:fa-file TNSNAMES.ora] & B02[fa:fa-folder-open Drivers] &     B03[fa:fa-folder-open SQLDeveloper] & B04[fa:fa-folder-open SQL Datamodeler]
  B02 --> B0201[fa:fa-file Drv-MySQL] & B0202[fa:fa-file Drv-PostGreSql]
```


### **Estrutura GitHub**

```mermaid
graph TD
A01[fa:fa-home github.com/conta/] --> C[fa:fa-folder-open repositório]
C --> C02[fa:fa-folder-open .devcontainer]
C --> C03[fa:fa-file .gitignore] & C04[fa:fa-file .gitattributes]
C --> C05[fa:fa-file .pre-commit-config.yaml]
C --> C10[fa:fa-file README.md]
C --> C11[fa:fa-file CODE_OF_CONDUCT.md]
C --> C12[fa:fa-file CONTRIBUTING.md]
C --> C19[fa:fa-file LICENSE.md]
C --> C13[fa:fa-file RELEASES.md]
C --> C14[fa:fa-file SECURITY.md]
C --> C31[fa:fa-file Dockerfile]
C --> D01[fa:fa-folder-open .github]
C --> D04[fa:fa-folder-open .github-private]
D04 --> SP0401[fa:fa-file README.md]
C --> D02[fa:fa-folder-open profile]
D02 --> SP01[fa:fa-file README.md]
C --> D03[fa:fa-folder-open workflow-templates]
D03 --> SP30[fa:fa-file template.yml] & SP31[fa:fa-file template.properties.json]
D01 --> SP11[fa:fa-file CODEOWNERS]
D01 --> SP12[fa:fa-folder-open workflows]
D01 --> SP13[fa:fa-folder-open ISSUE_TEMPLATE]
SP12 --> SP1201[fa:fa-file actions.yml]
SP13 -->SP1301[fa:fa-file bug_report.md]
SP13 -->SP1302[fa:fa-file feature_request.md]
SP13 -->SP1303[fa:fa-file config.yml]
C --> D10[fa:fa-folder-open docs]
C --> D11[fa:fa-folder-open iac]
C --> D12[fa:fa-folder-open front-end]
C --> D13[fa:fa-folder-open back-end]
D12 --> D1201[fa:fa-folder-open src]
D1201 --> D120101[fa:fa-folder-open main]
D1201 --> D120102[fa:fa-folder-open test]
```


```mermaid
mindmap
  root((repositorio))
    Monolito
      RepositorioAPP
         README.md
         package.json
         utils
           DigitoCpf.java
         libs
           jdbc.jar
         Documentacao
           Excel
           Word
    Monorepo
      Repositorio
        diretorioshared
        diretorioapps
        package.json
        webpack.config.js
        yarn.lock
    Polyrepo
      RepositorioDocumentacao
         Excel
         Word
      RepositorioFrontEnd
         html
         css
         js
      RepositorioBackEnd
         java
            src
            test

```

```mermaid
flowchart TD
    id1(main) --> id2(wip/tipos-nnnn)
    id2 --> id3(Pull Request)
    subgraph CI
      direction TB
      subgraph Pull Request Validação
        direction LR
        PRV00(Pretty) --> PRV01(Linter)
        PRV01         --> PRV02(Security Scanner)
        PRV02         --> PRV03(Teste Unitário)
        PRV03         --> PRV04(Covarage)
        PRV04         --> PRV05(PR Review)
      end
    end
    subgraph CD
      direction TB
      subgraph Release
       cd1(Git Tag</br>Version) -->cd2(Deploy to </br>Stage)
       cd2 --> cd3(Release)
      end
    end
    id3    --> CI
    CI     --> cd4(Squash<br/>merge)
    cd4    --> SAST01(SAST</br>BOM)
    CI     --> SAST02(SAST</br>RUIM)
    SAST01 --> CD
    subgraph Stage
      direction TB
      subgraph SIT
         sit01(Virtual Machine)
         sit02(Container)
         sit03(APP Service)
      end
      subgraph PRD
         prd01(Virtual Machine)
         prd02(Container)
         prd03(APP Service)
      end
    end
    CD --> Stage

```


### Centralização de Logs

```mermaid
graph LR
    Computador-A[Computador] -->|Syslog| B[Syslog Server]
    Computador-B[Computador] -->|Syslog| B[Syslog Server]
    Computador-C[Computador] -->|Syslog| B[Syslog Server]
```



```mermaid
graph TD
    subgraph Sistemas Operacionais
        Linux[[Linux<br>rsyslog/syslog-ng]]
        Windows[[Windows<br>Event Viewer/Winlogbeat]]
    end

    subgraph Servidores Aplicação
        Tomcat[[Tomcat<br>catalina.out]]
        JBoss[[JBoss<br>server.log]]
    end

    subgraph Aplicações Customizadas
        App1[[App Java<br>Log4j/Logback]]
        App2[[.NET App<br>Serilog/NLog]]
    end

    subgraph Coleta
        Filebeat -->|Coleta logs| Logstash
        Fluentd -->|Agrega dados| Kafka
        Winlogbeat -->|Eventos Windows| Logstash
        Rsyslog -->|Encaminha logs| Logstash
    end

    subgraph Processamento
        Logstash[[Logstash<br>Filtragem/Enriquecimento]]
        Kafka[[Kafka<br>Buffer de Mensagens]]
    end

    subgraph Armazenamento
        Elasticsearch[(Elasticsearch<br>Indexação)]
        S3[[AWS S3/Glacier<br>Backup Frio]]
    end

    subgraph Visualização & Gestão
        Kibana[[Kibana<br>Dashboards]]
        Grafana[[Grafana<br>Monitoramento]]
        Alertas[[ElastAlert<br>Notificações]]
    end

    Linux -->|syslog| Rsyslog
    Windows -->|Eventos| Winlogbeat
    Tomcat -->|Log Files| Filebeat
    JBoss -->|Log Files| Filebeat
    App1 -->|Log Files| Filebeat
    App2 -->|Log Files| Filebeat

    Rsyslog --> Logstash
    Winlogbeat --> Logstash
    Filebeat --> Logstash
    Logstash --> Kafka
    Kafka --> Elasticsearch
    Elasticsearch --> Kibana
    Elasticsearch --> Grafana
    Elasticsearch --> S3
    Kibana --> Alertas
```



## **maven-archetype-archetype** (Para criar novos archetypes)

```mermaid
graph TD
    A[archetype] --> B[src/main/resources/archetype-resources]
    B --> C[pom.xml]
    B --> D[src/main/java]
    B --> E[src/test/java]
    A --> F[src/main/resources/META-INF/maven/archetype-metadata.xml]
```

###  **maven-archetype-j2ee-simple** (Projeto J2EE básico)


```mermaid
graph TD
    A[project] --> B[ejb-module]
    A --> C[war-module]
    B --> D[src/main/java]
    B --> E[pom.xml]
    C --> F[src/main/webapp/WEB-INF]
    C --> G[pom.xml]
    A --> H[pom.xml]
```

### **maven-archetype-plugin** (Plugin Maven)

```mermaid
graph TD
    A[plugin-project] --> B[src/main/java/.../Mojo.java]
    A --> C[src/test/java]
    A --> D[pom.xml]
    A --> E[src/main/resources/META-INF/maven/plugin.xml]
```

### **maven-archetype-plugin-site** (Site para plugins)

```mermaid
graph TD
    A[plugin-site] --> B[src/site/apt]
    B --> C[example.apt]
    A --> D[pom.xml]
    A --> E[src/site/site.xml]
```

### **maven-archetype-portlet** (Portlet JSR-268)

```mermaid
graph TD
    A[portlet] --> B[src/main/webapp/WEB-INF]
    B --> C[portlet.xml]
    B --> D[web.xml]
    A --> E[pom.xml]
    A --> F[src/main/java]
```

### **maven-archetype-quickstart** (Projeto Java simples)

```mermaid
graph TD
    A[quickstart] --> B[src/main/java/App.java]
    A --> C[src/test/java/AppTest.java]
    A --> D[pom.xml]
```

### **maven-archetype-site** (Site documentation)
```mermaid
graph TD
    A[site] --> B[src/site/apt]
    B --> C[index.apt]
    A --> D[pom.xml]
    A --> E[src/site/site.xml]
```

### **maven-archetype-webapp**

```mermaid
graph TD
    A[webapp] --> B[src/main/webapp]
    B --> C[WEB-INF/web.xml]
    B --> D[index.jsp]
    A --> E[pom.xml]
    A --> F[src/main/java]
```
