### Seguindo os passos do curso FastAPI
[FastAPI](https://fastapi.tiangolo.com/)

### Habilitar o ambiente virtual para que o poetry enxergue as dependencias

poetry shell

### Iniciar a aplicação
fastapi dev meuarquivo.py


### Parar reconhecer o autocomplete do vscode
* $ poetry new eridanus 
* $ cd eridanus/
* $ python -m venv .venv
* $ poetry shell

### Configurando o Banco de Dados e Gerenciando Migrações com Alembic

* O SQLAlchemy é um exemplo de ORM. Ele permite que você trabalhe com bancos de dados SQL de maneira mais natural aos programadores Python. Em vez de escrever consultas SQL cruas, você pode usar métodos e atributos Python para manipular seus registros de banco de dados. Importar o SQLAlchemy **poetry add sqlalchemy**

* pydantic-settings: Serve para gerenciar nossas configurações de ambiente. A biblioteca permite que você defina configurações em arquivos separados ou variáveis de ambiente e acesse-as de uma maneira estruturada e segura em seu código. Importar o pydantic-settings **poetry add pydantic-settings**


### Alembic
* é uma ferramenta de migração de banco de dados para SQLAlchemy
* Após a instalação do Alembic, precisamos iniciá-lo em nosso projeto. O comando de inicialização criará um diretório migrations e um arquivo de configuração alembic.ini
* alterar o arquivo migrations/env.py para entender o projeto mapeado
* depois executar o código ***alembic revision --autogenerate -m "create users table"***
