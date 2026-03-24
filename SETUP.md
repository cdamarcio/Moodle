Guia de Instalação e Configuração (SETUP)

Este guia orienta a configuração do ambiente de desenvolvimento local.

1. Pré-requisitos

Antes de começar, certifique-se de ter instalado:

Python 3.11+

Docker e Docker Compose

Git

2. Configuração do Ambiente Python

Clone o repositório:

git clone [https://github.com/seu-usuario/moodle-clone.git](https://github.com/seu-usuario/moodle-clone.git)
cd moodle-clone


Crie um ambiente virtual:

python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate


Instale as dependências:

pip install -r requirements.txt


3. Configuração da Base de Dados (Docker)

O projeto utiliza PostgreSQL. Para subir o serviço:

docker-compose up -d db


4. Migrações e Dados Iniciais

Execute as migrações:

python manage.py migrate


Crie um super-utilizador (Administrador):

python manage.py createsuperuser


5. Executar o Servidor

python manage.py runserver


O sistema estará disponível em http://localhost:8000.
