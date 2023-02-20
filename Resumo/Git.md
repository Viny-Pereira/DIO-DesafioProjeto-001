Até o momento foram apresentados uma série de informações sobre o funcionamento interno por trás do Git, além de informações sobre o GitHub.

Para realizar as requisições e envios de arquivos para o servidor é necessário que haja um email e nome de usuários cadastrados, recomenda-se que use as mesmas informações do GitHub.
- Configurar nome de usuário

`git config --global user.name "name"`

- Configurar email 

`git config --global user.mail "mail"`

Para maior segurança recomenda-se a vinculação de uma chave SSH, para o dispositivo de confiança que você pretende usar, pois representa uma maior segurança e tira a necessidade de utilização de autenticação por email e senha

Inialização do repositorio local

`git init`

Atualizar informações do repositório 

`git add "nome do arquivo"`

Confirmar atualização de dados e enviar para o "servidor" local

`git commit -m "your commit"`

Enviar para o servidor 

`git push "URL do servidor" master` 

- Determinar um nome a url do servidor para facilitar o processo

`git remote add origin "URL do servidor"`
