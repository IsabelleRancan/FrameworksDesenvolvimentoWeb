FRAMEWORKS DESENVOLVIMENTO WEB

-> Nesta matéria vamos utilizar a linguagem: Python e o framework Flask; 
-> ORM - Mapeamento de Objeto Relacional: SQLAlchemy;

AULA 01 (09/10):
ANOTAÇÕES E FORMAS DE AVALIAÇÃO 

    Avaliação:
        1- Programação ao vivo (vamos receber o pedido 48h antes) - (11 e 18/12)
        2- Entrega do portifólio; (12/02)
        3- Aplicação prática com requisitos (22/01)
        vai ser a última atividade, precisa ter:
        pelo menos uma API desenvolvida por mim;
        tem que ter um end point documentados com períodos de entrada e saída;
        código limpo (nada de linhas de comentário);
        funcionando;
        com validações necessárias como entrada de dados, erro etc;
        BONUS se for uma aplicação elástica ou escalável;
        Tem que ter integração com banco de dados; 
        Os testes vão ser feitos seguindo a nossa documentação do projeto;
        Individual. 

    Revisar para a próxima aula:
        Criar um ambiente virtual do python com VENV (descobrir como criar pelo terminal tbm);
        Estar famiiarizado com linux...;
        Saber instalar pacote no Python;
        Extensões do Python - Python Venv (f1 e digitar create... criar ambiente virtual, criar um venv na minha versão do python), vai criar uma pasta oculta na pasta onde estou;
        executar o activate que tá na pasta;
        Vamos instalar pacotes para podermos usar nas aulas; 
        Requiriments - arquivo de dependências para replicar o ambiente virtual. É um arquivo TXT que vem com as dependencias que usamos + a versão; (é tipo packet json)
        -> dá pra gerar pelo próprio Python;
        Descobrir como gerar e usar pra poder testar;

    O python 3.11 pelo menos deve estar instalado na máquina; 

    SABER USAR LINUX!  

    Boas práticas:
        Nunca colocar código dentro da pasta do ambiente virtual;

    Aplicações WEB e não locais; 

AULA 2 (23/10):
CRIANDO UM AMBINETE VIRTUAL EM PYTHON:

    Passo a passo:
        - Criando o ambiente dentro do terminal do VSCode: python -m venv nome_do_ambiente
        - Autorizar a criação dos ambinetes (dentro do powershell) - necessário apenas 1 vez: 
            Get-ExecutionPolicy
            Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
        - Ativando o ambiente: nome_do_ambiente\Scripts\activate

        Para acessar venv depois de criado: 
        - Acessando o caminho: cd D:\Documentos Usuário\Documents\GitHub\FrameworksDesenvolvimentoWeb\projeto01
        - Ativando: ambiente1.venv\Scripts\activate
        - Desativando: deactivate

    Instalando dependencias:
        pip install nome_pacote
        pip list - exibe todos os pacotes instalados
    -> O que instalamos nessa primeira aula:
            flask
            flask sqlalchemy
            numpy - serve para manipular arrays, matrizes etc, é mais rápido que laços de repetição
    -> pypi - site que tem campo de busca de pacotes e como instalar.

    INSTALAMOS E RODAMOS BIBLIOTECAS SEMPRE DENTRO DO AMBIENTE VIRTUAL

    -> Nesta aula criamos as pastas: templates, static e pastas adjacentes. Além disso, o arquivo app.py - app.py é o arquivo principal que vamos utilizar;
    -> Utilizamos a barra de progresso e o tempo.

    * As aulas vão começar com uma lista de atividades, depois conceitos que vamos utilizar pra fazer essas atividades.

* PADÕRES DE ARQUIVO E ORGANIZAÇÃO DE CÓDIGO:
    - Frameworks trabalham com padrão;
    - Os arquivos html devem estar na pasta templates nessa primeira parte;
    - CÓDIGO LIMPO! ZERO COMENTÁRIOS E NOMES RELEVANTES; 
    - NOMES TODOS EM INGLÊS, NADA EM PORTUGUÊS - classes, variáveis, nomes, arquivos;
    - Variáveis snakecase (padrão da linguagem), nada de acentos ou caracteres especiais.