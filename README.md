![Imersão Full Stack && Full Cycle](https://events-fullcycle.s3.amazonaws.com/events-fullcycle/static/site/img/grupo_4417.png)

Participe gratuitamente: https://imersao.fullcycle.com.br/

# Vídeo:

## Sobre o repositório
Esse repositório contém o código-fonte ministrado na aula Django - Desenvolva grandes aplicações em minutos [https://www.youtube.com/watch?v=NC6aUo5rxco](https://www.youtube.com/watch?v=NC6aUo5rxco)

## Assistido até: 1:30:10 ->  https://youtu.be/NC6aUo5rxco?t=5574

https://github.com/professorsoares/live-imersao-fullcycle11-django

## Rodar a aplicação

O projeto foi construído com o VSCode + Dev Container(Extension), com eles você poderá rodar facilmente sem mesmo executar nenhum comando Docker.

Aplique o atalho `CTRL+SHIFT+P` VSCode e selecione a opção: 'Open Folder In Container'. O VSCode vai recarregar, levantar o container e instalar a extensão do Python. Aguarde alguns segundos e abra o terminal do VSCode e digite os seguintes comandos:


```bash
python manage.py migrate
python manage.py loaddata initial_data
```

Acesse a aplicação em [http://localhost:8000/admin](http://localhost:8000/admin)

Usuário para login:

```bash
username: admin@user.com
password: secret
```
ver

-----------------------------------------

# PASSO A PASSO:

## No Linux:

- Abra o Linux no windows;
- Inicialize o docker:  sudo dockerd
- Vá na pasta do projeto e abra o VSCode: ~/git/fullcycle/django/live-imersao-fullcycle11-django$ code .

## No VSCode:

- Aperte "Ctrl + Shift + p" -> Escolha a opção Dev Containers: "Open folder in Container"
- Escolha a pasta do código.
- Aperte "Ctrl + '" para ter o foco no terminal.
- Ative o Virtual Enviroment com o comando:         

```bash 
pipenv shell
```
- Rode o Comando:                                   
```bash 
python manage.py migrate
```
- Execute o Servidor do Django:                     
```bash
python manage.py runserver 0.0.0.0:8080
```
- Se fizer ajustes nos Models que afetem a base, rodar o comando:       
```bash
python manage.py makemigrations
```

### Para inserir no CRUD pelo TERMINAL
- Aperte Ctrl + "'" para  ir para o terminal
- Rode o Comando: 
```bash
python manage.py shell
```

EXEMPLO: 
- Importe o model desejado: 
```bash
from app.models import Player
```
- Crie o objeto: 
```bash
Player.objects.create(name='Bruno Augusto', initial_price=20000)
```

### Para fazer backup e recuperar os dados de backup
- Para bkp dos dados das tabelas de cada módulo, rode o comando:    
```bash
python manage.py dumpdata app
```
- Para bkp dos dados das tabelas de auth, rode o comando:           
```bash
python manage.py dumpdata auth
```


### GIT
- Para criar um novo repositório no git rode os comandos:
- - wewe

## Definições:
- O arquivo "admin.py" é onde definimos as configurações para apresentação do Admin.
- O arquivo "models.py" é onde definimos os modelos(Objetos) que serão migrados para o Banco de Dados, com seus respectivos relacionamentos.
- 
