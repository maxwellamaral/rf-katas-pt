# Começando

Nesta seção, instalaremos o Robot Framework, as bibliotecas de teste necessárias e garantiremos que o ambiente esteja
funcionando para fazer testes de interface do usuário da Web com o Robot Framework.

## Terminologia

Nesta seção, você verá muitos jargões relacionados ao Python, ao sistema operacional e ao Robot Framework que podem ser
confusos para alguns. Portanto, antes de prosseguir, vamos esclarecer algumas terminologias que são usadas com
frequência nesse ecossistema.

- *pip* - Gerenciador de pacotes Python, esta é uma ferramenta necessária para instalar o Robot Framework e as
  bibliotecas de teste necessárias
- *shell* - O shell é o interpretador de comandos em um sistema operacional como Unix ou GNULinux, é um programa que
  executa outros programas
- *bat / batch file / cmd* - Um arquivo de lote é um arquivo de script no DOS, OS2 e Microsoft Windows. Consiste em uma
  série de comandos a serem executados pelo interpretador de linha de comando, armazenados em um arquivo de texto
  simples.
- *robot* - A ferramenta de linha de comando que permite ao usuário executar casos de teste e tarefas do Robot Framework
- *test suite* - Um arquivo Robot que contém casos de teste
- *keyword* - um componente, semelhante a uma função na programação, que o robô usa para executar etapas
- *arguments* - Valores que são dados a palavras-chave. Também conhecido como parâmetros.

## Obtenha o Repositório

Clone o repositório ou baixe e extraia o ZIP do repositório para sua máquina local. Todos os exercícios serão concluídos
usando a cópia local do repositório.

![Clonar o repositório](img/clone_repo.png)

## Instalar o Robot Framework

Para executar os casos de teste do Robot Framework, precisaremos instalar o Robot Framework. Nós instalamos isso
usando `pip`. Por padrão, a instalação acontece chamando `pip3 install <package_name>`, mas se você estiver usando um
ambiente virtual, ou tiver um alias definido, você pode tentar `pip install <package_name>` em vez disso.

Instale o Robot Framework: `pip3 install robotframework`.

Se a instalação foi bem-sucedida, você pode usar o comando `robot -h` para verificar se obteve ajuda da linha de comando
para o Robot Framework. A saída deve incluir o número da versão do robô e algumas outras coisas úteis, incluindo as
opções de linha de comando (que também estão disponíveis
em [aqui](http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#all-command-line-options)).

Para executar casos de teste automatizados para UIs da Web, a biblioteca atual é a Browser-library.

Instale o navegador: `pip3 install robotframework-browser`. Após a instalação ser concluída com sucesso, a biblioteca
deve ser inicializada executando `rfbrowser init`.

Para garantir que você tenha feito os exercícios conforme o esperado, precisamos que você instale a ferramenta
robotframework-lint. Uma ferramenta de linting é uma ferramenta de análise estática leve para verificar se você e sua
equipe estão fazendo seu código de forma consistente.

Install Robot Framework linter: `pip3 install robotframework-lint`.

## Instalar o NodeJS

A biblioteca do navegador tem requisitos para NodeJS. Após instalar o NodeJS, execute o comando: `rfbrowser init` para
instalar as dependências necessárias.

## Iniciar servidor

Para executar os exercícios deste treinamento, você precisa iniciar o aplicativo de demonstração. Você pode iniciar o
servidor executando `python3 server/server.py` no prompt de comando do terminal. Seu terminal ou prompt de comando agora
está ocupado com a execução do servidor, o que significa que você precisa abrir outro prompt de comando do terminal para
executar seus testes.

Depois que o servidor for iniciado, ele será executado em http:localhost:7272.

## Verifique a instalação

Verifique a configuração executando:

- no Windows: execute o comando `python verify.py 00`
- no macOSLinux: execute o comando `python3 Verify.py 00`

Isso deve levar alguns segundos. Se a saída do script terminar com `Setup in perfect condition!`
estamos prontos para ir.

Caso contrário, verifique a saída e corrija os pacotes ausentes.
