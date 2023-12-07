# Guia Virtual Envs

## Introduzindo as Venvs

### O que é uma Venv
Virtual Envs são ambientes virtuais usados para isolar um projeto do sistema, com elas é possível isolar as dependências e usar versões diferentes do Python, o que possibilita realizar testes isolados, evitando conflitos entre pacotes e versões.

### Como funcionam 
Ao criar uma Venv, é criada uma pasta que contém uma cópia do Python padrão do sistema, contendo os arquivos e pacotes default do Python. A instalação dos pacotes é exclusivamente feita na pasta da Venv, isoladamente das outras Venvs e dos pacotes instalados no sistema. Cada Venv é relacionada a um projeto.

### Tipos de Venvs
Desde a versão 3.3, o [venv](https://docs.python.org/3/library/venv.html) vem por padrão na instalação do Python, este é o modo mais simples de criar uma Venv, todos os pacotes são instalados através do [pip](https://pypi.org/project/pip/). Existem outros pacotes para manipular Venvs, como exemplo o [virtualenv](https://virtualenv.pypa.io/en/latest/) que é uma versão mais completa do venv, e o [pyenv](https://github.com/pyenv/pyenv) que é mais usado para criação de Venvs usando diferentes versões do Python. Outra ferramenta que pode ser usada é o Poetry, que gerencia as dependências e os pacote de um projeto usando Venvs, facilitando e organizando o processo. Saiba mais em [python-poetry.org](https://python-poetry.org/) 
## Manipulando Venvs

### Criando e ativando uma Venv
Inicialmente, para criar uma Venv basta usar `python -m venv nome-da-pasta`, será criada uma pasta dentro do diretório do projeto com o nome informado. Para acessar a Venv é preciso ativá-la usando   `.\nome-da-pasta-da- venv\Scripts\activate`. Após isso a Venv está pronta para ser usada, basta instalar os pacotes desejados e executar o projeto normalmente `python nome-do-arquivo.py`.

### Desativar e excluir uma Venv
As Venvs podem ser desativadas usando `deactivate` e reativadas normalmente. Em outros casos para excluir uma Venv basta excluir a pasta referente no diterório do projeto.

## Documentações

[docs.python.org/venv](https://docs.python.org/3/library/venv.html#creating-virtual-environments)

[virtualenv.pypa.io](https://virtualenv.pypa.io/en/latest/)

[github.com/pyenv](https://github.com/pyenv/pyenv)