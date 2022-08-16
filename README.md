# Robot Framework katas

## Requisitos

Nesta série de exercícios vamos executar vários testes automatizados em uma aplicação web. Para isso, precisaremos ter
os seguintes itens instalados:

- Python (versão 3.7 ou mais recente): https://www.python.org/downloads/
    - Lembre-se de adicionar a pasta Python à variável de ambiente PATH.
- Pip for Python 3
    - Windows: https://www.howtogeek.com/197947/how-to-install-python-on-windows/
    - Linux: `sudo apt-get install python3-pip && pip3 install --upgrade pip`
    - macOS: `brew install python` pip já está incluído
- Node.js (versão 12 ou mais recente): https://nodejs.org/en/download/
- Sistema em teste
    - Abra uma nova janela de terminal, altere o diretório para esta pasta raiz do repositório e execute o aplicativo
      com: `python server/server.py`

### Recomendado

- Para facilitar a instalação com pip, use virtualenv (https://virtualenv.pypa.io/en/latest/)
    - Instruções curtas para uso do virtualenv

      ```shell
      pip install virtualenv --user
      virtualenv <choose_a_folder_name>
      source <chosen_folder_name>/bin/activate
      ```

## Iniciar

Depois de instalar os requisitos, verifique o [Começando o exercício](exercises/00-getting-started.md) e prossiga com os exercícios.
