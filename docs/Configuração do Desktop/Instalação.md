# Base de Instalação

## IDE

```
 $ [MELD](https://meldmerge.org/).   # Visual diff and merge tool
 $ [VSCode](https://code.visualstudio.com/download)
```

## Gerenciamento de Pacotes

```
$ brew install maven
$ brew install deno
$ brew install node
$ brew install composer
```

## Texto

```
$ brew install figlet      # Palavra em Arquivos de Texto
```

## Zsh

```
$ brew install zsh
```

## Teste

```
$ brew install jmeter
$ Selenium WebDriver
$ brew install k6
$ Gatling (https://gatling.io/)
$ npm install cypress --save-dev
$ brew install allure
$ Insonia
$ Postman
$ Jest
$ Testify
$ PHPUnit
$ Pest
$ Mocha
$ Chrome DevTools
$ Firefox Developer Tools
$ Lighthouse
$ JUnit
$ Mockito
```

## Cobertura de Código

```
$ JaCoCo
```
## Container

```
$ Docker 
$ Docker Compose
```

## Monitoramento

```
$ Prometheus
$ Grafana
$ SigNoz
```
## Git

```
$ brew install git          #
$ brew install git-flow     #
$ brew install git-lfs      #
$ brew install git-secrets  # 
$ brew install gitleaks     # senhas,chaves API, tokens repositório   
$ brew install pre-commit   #  
$ brew install osv-scanner  # Vulnerabilidades dependências do seu projeto
$ brew install gh           # GitHub CLI
$ brew install act          # GitHub Actions CLI
```
## Maven

```
$ brew install maven        #
```

## Python

```
$ ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"
$ brew install python       #    
$ brew install python3      #
```
## Pip
 ```
 $ pip list                         #
 $ pip install -r requirements.txt  #
 ```

## Terraform
```
$ brew tap hashicorp/tap                #
$ brew install hashicorp/tap/terraform  #
$ brew update                           #
```

## Ansible

```
$ brew install ansible                  #
```

## Cosign

```
$ brew install cosign                  # Assinatura de Container
```

## Linters

```
$ npm i eslint
$ GoLang: curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/HEAD/install.sh | sh -s -- -b $(go env GOPATH)/bin v2.1.2
$ PHP: curl -OL https://squizlabs.github.io/PHP_CodeSniffer/phpcs.phar
$ PHP: curl -OL https://squizlabs.github.io/PHP_CodeSniffer/phpcbf.phar
```

## Listar Instalação

```
$ brew list                      # Listar pacotes instalados
$ pip list                       # Listar pacotes instalados
$ code --list-extensions         # Listar extensão vscode
$ pip list | awk 'NR>2 { printf "%-30s %-20s ", $1, $2 } (NR-4) % 4 == 0 { print "" } END { if ((NR-4) % 4 != 0) print "" }'
$ pip list | tail -n +6 | paste - - | column -t
```

# Ferramentas de Produtividade
## Oracle

```
$ SQL Developer   # Ferramenta acesso ao Banco de Dados
$ SQL Datamodeler # Ferramenta de Modelagem de Dados DER/MER Conceitual
```
## JSON/XML

```
$ brew install jq # Processador de linha de comando JSON
$ brew install yq # Processador de linha de comando YAML, JSON e XML
```

# Ferramentas de Documentação

```
 $ Download [obsidian](https://help.obsidian.md/install)
 $ cargo binstall marmite
 $ pip install mkdocs
 $ Download [VsCode](https://code.visualstudio.com/download)
 $ [Swagger](https://editor.swagger.io/)
 $ [JSDoc/TSDoc](https://jsdoc.app/)
 $ [PL/Doc](https://jsdoc.app/)
 ```
## Instalação de Pacotes ou Configurações

### Configuração Git

```
-- Caso você possua inúmeras contas
[include]
path = ~/gitconfig/.gitconfig_github_xxxxxx
path = ~/gitconfig/.gitconfig_gitlab_xxxxxx
path = ~/gitconfig/.gitconfig_person_xxxxxx
path = ~/gitconfig/.gitconfig_azure_xxxxxxxx

[core]
        editor = code --wait
        excludesfile = $HOME/gitconfig/.gitignore_global
        quotepath = false
        hooksPath = $HOME/gitconfig/hooks
[commit]
        template = $HOME/gitconfig/mensagem/.commitmensagem
        gpgsign = true
[sendemail]
        smtpEncryption = tls
        confirm = auto
        smtpServer = smtp.gmail.com
        smtpUser = usuario@gmail.com
        smtpServerPort = 587
        smtppass = "******"
        suppresscc = self
        transferEncoding = "8bit"
[changelog]
        format = "%x09 %ad %d %s (%aN)"
        mergeformat = ' * %s%n%w(64,4,4)%b'
[difftool]
        prompt = false
[difftool "meld"]
        cmd = meld "$LOCAL" "$REMOTE"
[difftool "sourcetree"]
        cmd = opendiff \"$LOCAL\" \"$REMOTE\"
        path =
[mergetool "sourcetree"]
        trustExitCode = true
[rerere]
        enabled = true
```

### Pip

```
Package                                   Version
----------------------------------------- --------------
aiofiles                                  24.1.0
aiohappyeyeballs                          2.4.4
aiohttp                                   3.11.11
aiosignal                                 1.3.2
alabaster                                 1.0.0
alembic                                   1.15.1
altair                                    5.5.0
annotated-types                           0.7.0
ansible                                   11.2.0
ansible-core                              2.18.2
anthropic                                 0.45.0
antlr4-python3-runtime                    4.9.3
anyio                                     4.8.0
appdirs                                   1.4.4
appnope                                   0.1.4
arrow                                     1.3.0
asgiref                                   3.8.1
asttokens                                 3.0.0
asyncer                                   0.0.8
attrs                                     25.1.0
av                                        13.1.0
azure-ai-textanalytics                    5.3.0
azure-ai-vision-imageanalysis             1.0.0
azure-common                              1.1.28
azure-core                                1.32.0
babel                                     2.16.0
backcall                                  0.2.0
backoff                                   2.2.1
backrefs                                  5.8
bcrypt                                    4.2.1
beautifulsoup4                            4.13.4
binaryornot                               0.4.4
bleach                                    6.2.0
blinker                                   1.9.0
bracex                                    2.5.post1
Brotli                                    1.1.0
build                                     1.2.2.post1
CacheControl                              0.14.2
cachetools                                5.5.1
cairocffi                                 1.7.1
CairoSVG                                  2.7.1
certifi                                   2024.12.14
cffi                                      1.17.1
cfgv                                      3.4.0
chardet                                   5.2.0
charset-normalizer                        3.4.1
chroma-hnswlib                            0.7.6
chromadb                                  0.6.3
chromedriver-binary                       134.0.6977.0.0
chromedriver-binary-auto                  0.3.1
cleo                                      2.1.0
click                                     8.1.8
click-man                                 0.5.0
cloudpickle                               3.1.1
cloup                                     3.0.5
colorama                                  0.4.6
coloredlogs                               15.0.1
contourpy                                 1.3.1
cookiecutter                              2.6.0
crashtest                                 0.4.1
cryptography                              44.0.0
csscompressor                             0.9.5
cssselect2                                0.7.0
cycler                                    0.12.1
Cython                                    3.0.11
databricks-sdk                            0.46.0
dataclasses-json                          0.6.7
decorator                                 5.1.1
deepdiff                                  8.1.1
defusedxml                                0.7.1
Deprecated                                1.2.17
detect-secrets                            1.5.0
diskcache                                 5.6.3
distlib                                   0.3.9
distro                                    1.9.0
dnspython                                 2.7.0
docker                                    7.1.0
docopt                                    0.6.2
docutils                                  0.21.2
dulwich                                   0.22.8
durationpy                                0.9
EditorConfig                              0.17.0
effdet                                    0.4.1
email_validator                           2.2.0
emoji                                     2.14.1
et_xmlfile                                2.0.0
eval_type_backport                        0.2.2
executing                                 2.2.0
fast-depends                              2.4.12
fastapi                                   0.115.7
fastapi-cli                               0.0.7
fastjsonschema                            2.21.1
filelock                                  3.17.0
filetype                                  1.2.0
findpython                                0.6.3
FLAML                                     2.3.3
Flask                                     3.1.0
Flask-DebugToolbar                        0.16.0
Flask-Login                               0.6.3
Flask-Mail                                0.10.0
flask-mongo-sessions                      0.2.1
flask-mongoengine                         1.0.0
Flask-PyMongo                             2.3.0
Flask-SQLAlchemy                          3.1.1
Flask-User                                1.0.2.2
Flask-WTF                                 1.2.2
flatbuffers                               25.1.24
fonttools                                 4.55.6
fpdf2                                     2.8.2
frozendict                                2.4.6
frozenlist                                1.5.0
fsspec                                    2024.12.0
ghp-import                                2.1.0
git-dummy                                 0.1.2
git-sim                                   0.3.5
git-story                                 0.1.4
git-tagup                                 0.1.2
gitdb                                     4.0.12
github3.py                                4.0.1
GitPython                                 3.1.44
glcontext                                 3.0.0
google-api-core                           2.24.0
google-auth                               2.38.0
google-cloud-vision                       3.9.0
googleapis-common-protos                  1.66.0
graphene                                  3.4.3
graphql-core                              3.2.6
graphql-relay                             3.2.0
greenlet                                  3.1.1
griffe                                    1.5.5
groq                                      0.15.0
grpcio                                    1.70.0
grpcio-status                             1.70.0
gunicorn                                  23.0.0
h11                                       0.14.0
hjson                                     3.1.0
html5lib                                  1.1
htmlmin2                                  0.1.13
httpcore                                  1.0.7
httptools                                 0.6.4
httpx                                     0.28.1
httpx-sse                                 0.4.0
huggingface-hub                           0.27.1
humanfriendly                             10.0
identify                                  2.6.6
idna                                      3.10
imageio                                   2.37.0
imagesize                                 1.4.1
importlib_metadata                        8.5.0
importlib_resources                       6.5.2
iniconfig                                 2.0.0
installer                                 0.7.0
iopath                                    0.1.10
ipython                                   8.12.3
isodate                                   0.7.2
isosurfaces                               0.1.2
itsdangerous                              2.2.0
jaraco.classes                            3.4.0
jaraco.context                            6.0.1
jaraco.functools                          4.1.0
jedi                                      0.19.2
Jinja2                                    3.1.5
jiter                                     0.8.2
joblib                                    1.4.2
jsbeautifier                              1.15.1
jsmin                                     3.0.1
jsonpatch                                 1.33
jsonpath-python                           1.0.6
jsonpointer                               3.0.0
jsonschema                                4.23.0
jsonschema-specifications                 2024.10.1
jupyter_client                            8.6.3
jupyter_core                              5.7.2
jupyterlab_pygments                       0.3.0
kaleido                                   0.2.1
keyring                                   25.6.0
kiwisolver                                1.4.8
kubernetes                                32.0.0
langchain                                 0.3.15
langchain-community                       0.3.15
langchain-core                            0.3.31
langchain-text-splitters                  0.3.5
langdetect                                1.0.9
langsmith                                 0.3.1
layoutparser                              0.3.4
lazy_loader                               0.4
libsass                                   0.23.0
lumache                                   0.0.0
lxml                                      5.3.0
Mako                                      1.3.9
manim                                     0.19.0
ManimPango                                0.6.0
mapbox_earcut                             1.0.3
Markdown                                  3.7
markdown-callouts                         0.4.0
markdown-include                          0.8.1
markdown-it-py                            3.0.0
MarkupSafe                                3.0.2
marshmallow                               3.26.0
matplotlib                                3.10.0
matplotlib-inline                         0.1.7
mdurl                                     0.1.2
mergedeep                                 1.3.4
mike                                      2.1.3
mistune                                   3.1.0
mkdocs                                    1.6.1
mkdocs-autorefs                           1.3.0
mkdocs-backlinks                          0.9.1
mkdocs-codeinclude-plugin                 0.2.1
mkdocs-exclude                            1.0.2
mkdocs-get-deps                           0.2.0
mkdocs-git-authors-plugin                 0.9.2
mkdocs-git-committers-plugin              0.2.3
mkdocs-git-committers-plugin-2            2.4.1
mkdocs-git-revision-date-localized-plugin 1.3.0
mkdocs-glightbox                          0.4.0
mkdocs-include-markdown-plugin            7.1.2
mkdocs-live-edit-plugin                   0.3.1
mkdocs-macros-plugin                      1.3.7
mkdocs-material                           9.6.11
mkdocs-material-extensions                1.3.1
mkdocs-mermaid2-plugin                    1.2.1
mkdocs-minify-plugin                      0.8.0
mkdocs-monorepo-plugin                    1.1.0
mkdocs-obsidian-bridge                    1.2.0
mkdocs-pdf-export-plugin                  0.5.10
mkdocs-print-site-plugin                  2.6.0
mkdocs-publisher                          1.4.7
mkdocs-redirects                          1.2.2
mkdocs-render-swagger-plugin              0.1.2
mkdocs-rss-plugin                         1.17.1
mkdocs-swagger-ui-tag                     0.6.11
mkdocs-table-reader-plugin                3.1.0
mkdocs-theme-topdf                        0.5.0
mkdocs-with-pdf                           0.9.3
mkdocstrings                              0.27.0
mkdocstrings-crystal                      0.3.7
mkdocstrings-python                       1.13.0
mlflow                                    2.21.0
mlflow-skinny                             2.21.0
mmh3                                      5.1.0
moderngl                                  5.12.0
moderngl-window                           3.1.1
mongoengine                               0.29.1
monotonic                                 1.6
more-itertools                            10.6.0
mpmath                                    1.3.0
msgpack                                   1.1.0
multidict                                 6.1.0
multipledispatch                          1.0.0
multitasking                              0.0.11
mypy-extensions                           1.0.0
narwhals                                  1.23.0
nbclient                                  0.10.2
nbconvert                                 7.16.5
nbformat                                  5.10.4
nest-asyncio                              1.6.0
networkx                                  3.4.2
nltk                                      3.9.1
nodeenv                                   1.9.1
numpy                                     2.2.2
oauthlib                                  3.2.2
obsidian-callouts                         1.0.1
obsidian-media                            2.0.0
olefile                                   0.47
ollama                                    0.4.7
omegaconf                                 2.3.0
onnx                                      1.17.0
onnxruntime                               1.20.1
openai                                    1.60.1
opencv-python                             4.11.0.86
opencv-python-headless                    4.11.0.86
openpyxl                                  3.1.5
opentelemetry-api                         1.29.0
opentelemetry-exporter-otlp-proto-common  1.29.0
opentelemetry-exporter-otlp-proto-grpc    1.29.0
opentelemetry-instrumentation             0.50b0
opentelemetry-instrumentation-asgi        0.50b0
opentelemetry-instrumentation-fastapi     0.50b0
opentelemetry-proto                       1.29.0
opentelemetry-sdk                         1.29.0
opentelemetry-semantic-conventions        0.50b0
opentelemetry-util-http                   0.50b0
ordered-set                               4.1.0
orderly-set                               5.2.3
orjson                                    3.10.15
outcome                                   1.3.0.post0
overrides                                 7.7.0
packaging                                 24.2
paginate                                  0.5.7
pandas                                    2.2.3
pandocfilters                             1.5.1
parso                                     0.8.4
passlib                                   1.7.4
pathspec                                  0.12.1
pbs-installer                             2025.3.17
pdf2image                                 1.17.0
pdfminer.six                              20231228
pdfplumber                                0.11.5
peewee                                    3.17.8
pexpect                                   4.9.0
pickleshare                               0.7.5
pika                                      1.3.2
pikepdf                                   9.5.1
pillow                                    11.1.0
pillow_heif                               0.21.0
pip                                       25.0.1
pip-tools                                 7.4.1
pipreqs                                   0.5.0
pkginfo                                   1.12.1.2
platformdirs                              4.3.6
playwright                                1.49.1
plotly                                    5.24.1
pluggy                                    1.5.0
poetry                                    2.1.1
poetry-core                               2.1.1
poppler-utils                             0.1.0
portalocker                               3.1.1
posthog                                   3.10.0
pre_commit                                4.1.0
prompt_toolkit                            3.0.50
propcache                                 0.2.1
proto-plus                                1.25.0
protobuf                                  5.29.3
psutil                                    6.1.1
ptyprocess                                0.7.0
pure_eval                                 0.2.3
pyaes                                     1.6.1
pyarrow                                   19.0.0
pyasn1                                    0.6.1
pyasn1_modules                            0.4.1
pyautogen                                 0.7.2
pycairo                                   1.27.0
pycocotools                               2.0.8
pycparser                                 2.22
pydantic                                  2.10.6
pydantic_core                             2.27.2
pydantic-settings                         2.7.1
pydeck                                    0.9.1
pydot                                     3.0.4
pydub                                     0.25.1
pydyf                                     0.11.0
pyee                                      12.0.0
PyGithub                                  2.5.0
pyglet                                    2.1.2
PyGLM                                     2.7.3
Pygments                                  2.19.1
PyJWT                                     2.10.1
pymdown-extensions                        10.14.1
pymongo                                   4.10.1
PyMuPDF                                   1.25.2
PyNaCl                                    1.5.0
pyobjc-core                               11.0
pyobjc-framework-Cocoa                    11.0
pypandoc                                  1.15
pyparsing                                 3.2.1
pypdf                                     5.1.0
pypdfium2                                 4.30.1
pyphen                                    0.17.2
PyPika                                    0.48.9
pyproject_hooks                           1.2.0
pyrr                                      0.10.3
PySocks                                   1.7.1
pytesseract                               0.3.13
pytest                                    8.3.4
pytest-base-url                           2.1.0
pytest-playwright                         0.6.2
python-dateutil                           2.9.0.post0
python-docx                               1.1.2
python-dotenv                             1.0.1
python-iso639                             2024.10.22
python-magic                              0.4.27
python-multipart                          0.0.20
python-oxmsg                              0.0.1
python-pptx                               1.0.2
python-slugify                            8.0.4
pytz                                      2024.2
PyYAML                                    6.0.2
pyyaml_env_tag                            0.1
pyzmq                                     26.2.0
RapidFuzz                                 3.11.0
referencing                               0.36.2
regex                                     2024.11.6
repo-activity-score                       0.0.4
requests                                  2.32.3
requests-oauthlib                         2.0.0
requests-toolbelt                         1.0.0
resolvelib                                1.0.1
rich                                      13.9.4
rich-toolkit                              0.13.2
rpds-py                                   0.22.3
rsa                                       4.9
safetensors                               0.5.2
scikit-image                              0.25.0
scikit-learn                              1.6.1
scipy                                     1.15.1
screeninfo                                0.8.1
selenium                                  4.28.1
setuptools                                75.8.0
shellingham                               1.5.4
six                                       1.17.0
skia-pathops                              0.8.0.post2
smmap                                     5.0.2
sniffio                                   1.3.1
snowballstemmer                           2.2.0
sortedcontainers                          2.4.0
soupsieve                                 2.6
Sphinx                                    8.1.3
sphinx-rtd-theme                          3.0.2
sphinxcontrib-applehelp                   2.0.0
sphinxcontrib-devhelp                     2.0.0
sphinxcontrib-htmlhelp                    2.1.0
sphinxcontrib-jquery                      4.1
sphinxcontrib-jsmath                      1.0.1
sphinxcontrib-qthelp                      2.0.0
sphinxcontrib-serializinghtml             2.0.0
SQLAlchemy                                2.0.37
sqlparse                                  0.5.3
srt                                       3.5.3
stack-data                                0.6.3
starlette                                 0.45.3
streamlit                                 1.41.1
super_collections                         0.5.3
svgelements                               1.9.6
sympy                                     1.13.1
tabulate                                  0.9.0
tach                                      0.23.0
Telethon                                  1.39.0
tenacity                                  9.0.0
termcolor                                 2.5.0
text-unidecode                            1.3
threadpoolctl                             3.6.0
tifffile                                  2025.1.10
tiktoken                                  0.8.0
timm                                      1.0.14
tinycss2                                  1.4.0
tinyhtml5                                 2.0.0
tokenizers                                0.21.0
toml                                      0.10.2
tomli                                     2.2.1
tomli_w                                   1.2.0
tomlkit                                   0.13.2
toolz                                     1.0.0
torch                                     2.5.1
torchvision                               0.20.1
tornado                                   6.4.2
tqdm                                      4.67.1
traitlets                                 5.14.3
transformers                              4.48.1
trio                                      0.28.0
trio-websocket                            0.11.1
trove-classifiers                         2025.3.19.19
typer                                     0.15.1
types-python-dateutil                     2.9.0.20241206
typing_extensions                         4.12.2
typing-inspect                            0.9.0
tzdata                                    2025.1
tzlocal                                   5.2
ujson                                     5.10.0
unstructured                              0.14.8
unstructured-client                       0.29.0
unstructured-inference                    0.7.36
unstructured.pytesseract                  0.3.13
uritemplate                               4.1.1
urllib3                                   2.3.0
uvicorn                                   0.34.0
uvloop                                    0.21.0
validators                                0.34.0
verspec                                   0.1.0
virtualenv                                20.29.1
watchdog                                  6.0.0
watchfiles                                1.0.4
wcmatch                                   10.0
wcwidth                                   0.2.13
weasyprint                                63.1
webdriver-manager                         4.0.2
webencodings                              0.5.1
websocket-client                          1.8.0
websockets                                14.2
Werkzeug                                  3.1.3
wheel                                     0.45.1
wrapt                                     1.17.2
wsproto                                   1.2.0
WTForms                                   3.2.1
xattr                                     1.1.4
xlrd                                      2.0.1
XlsxWriter                                3.2.1
yamllint                                  1.35.1
yarg                                      0.1.9
yarl                                      1.18.3
yfinance                                  0.2.52
zipp                                      3.21.0
zopfli                                    0.2.3.post1
zstandard                                 0.23.0
```

### VS Code

```
aldijav.golangwithdidi
bierner.markdown-mermaid
claudineyqr.plantuml-snippets
clysto.plantuml
coder.coder-remote
docker.docker
dotjoshjohnson.xml
doublebot.doublebot
douglaszaltron.nunjucks-vscode-extensionpack
esbenp.prettier-vscode
ex3ndr.llama-coder
formulahendry.code-runner
github.codespaces
github.copilot
github.copilot-chat
github.vscode-codeql
github.vscode-github-actions
github.vscode-pull-request-github
glenn2223.live-sass
golang.go
hediet.vscode-drawio
honnamkuan.golang-snippets
jebbs.plantuml
jme797.prettier-vscode-extension
mebrahtom.plantumlpreviewer
meezilla.json
mermaidchart.vscode-mermaid-chart
mohsen1.prettify-json
ms-azuretools.vscode-docker
ms-ceintl.vscode-language-pack-pt-br
ms-python.debugpy
ms-python.python
ms-python.vscode-pylance
ms-vscode-remote.remote-containers
ms-vscode-remote.remote-ssh
ms-vscode-remote.remote-ssh-edit
ms-vscode.powershell
ms-vscode.remote-explorer
ms-vsliveshare.vsliveshare
mushan.vscode-paste-image
neonxp.gotools
nhoizey.gremlins
oracle.sql-developer
oscarback.actions-to-graph
premparihar.gotestexplorer
qhoekman.language-plantuml
quicktype.quicktype
redhat.vscode-yaml
reditorsupport.r
ronnidc.nunjucks
shd101wyy.markdown-preview-enhanced
sidiandi.plantuml-sidiandi-fork
systemticks.c4-dsl-extension
teamsdevapp.ms-teams-vscode-extension
teamsdevapp.vscode-adaptive-cards
wakatime.vscode-wakatime
well-ar.plantuml
yzhang.markdown-all-in-one
zainchen.json
zxh404.vscode-proto3
```
