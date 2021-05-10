# Web app de Teoria da Computação
Web App base em Django para website de Teoria da Computação

### Passos para lançar e editar a aplicação
1. Abra a linha de comandos (PowerShell ou cmd)
1. Descarregue uma cópia (clone) do repositório com o comando `git clone https://github.com/teoria-da-computacao/tc-django` ou descarregue o projeto como um zip e descompacte
1. Entre na pasta  `cd tc-django`
2. Crie e instale um ambiente virtual. Use o venv ou o pipenv.
3. Instale o pipenv `python -m pip install pipenv`
4. Crie um ambiente virtual com o django instalado `pipenv install django`
5. Instale o graphviz `pipenv install graphviz`
6. Active o ambiente virtual `pipenv shell`
7. Lance a aplicação no browser com o comando `python manage.py runserver`
8. abra a pasta com o Pycharm, ou com o comando `pycharm .`

### Passos para criar uma nóva página na aplicação
1. no ficheiro `views.py` crie uma nova função que renderize a nova página
2. na pasta `website\templates\website` crie uma página HTML correspondente para ser renderizada, extendendo o layout base (veja como é feito nas outras páginas)
3. no ficheiro `website\urls.py` crie um novo `path` para o novo URL
4. no ficheiro `layout.html` (que está na pasta `website\templates\website`) atualize o menu de navegação, inlcuindo um link para a nova página
