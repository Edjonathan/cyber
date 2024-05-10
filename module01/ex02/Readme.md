Server-Side Request Forgery (SSRF)


Descrição

É um ataque que explora vulnerabilidades da aplicação tentando se aproveitar de inputs não tratados do sistema para realizar requests em seu nome. 
Em geral, quando a aplicação busca dados a partir de suas entradas, o atacante vai tentar alterar esses parametros para tentar forçar a aplicação
a realizar requisições orientados por ele.


Local File Inclusion

Descrição

É um ataque que explora vulnerabilidades da aplicação tentando se aproveitas de inputs não tratados, em sistemas que realizam upload de arquivos
no servidor. Quando o sistema de inputs recebe os paths e não tratam o atacante pode passar um path para um arquivo sensivel e obter dados desse
arquivo. 



Cenário de Sucesso:

Atacante conseguir enviar um path para o site e obter informações sensiveis do servidor que possibilite ele explorar o servidor e forçar a aplicação
executar requests para outros sistemas



Cenário Reais

1) Obtenção de dados sensiveis do servidor e conexão com um redis ou banco de dados da aplicação
2) Obtenção de informações sensiveis da aplicação, ex: metadados da aplicação



ref:
https://medium.com/alan/ssrf-in-real-life-3ef894d1f3be
https://rodolfomarianocy.medium.com/ssrf-entenda-o-b%C3%A1sico-de-forma-simples-e-algumas-formas-de-bypass-e694751acc0e
https://cheatsheetseries.owasp.org/cheatsheets/Server_Side_Request_Forgery_Prevention_Cheat_Sheet.html
https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Server%20Side%20Request%20Forgery/README.md