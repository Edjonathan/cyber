
Template Injection


Descrição

É um ataque que explora vulnerabilidades na aplicação na validação dos valores de input. Quando não há validação,
sanitização e tratativas adequadas nos inputs dos templates, os atacantes podem inserir códigos para serem executados no backend
que comprometa a aplicação. Ex: Usuário pode passar comandos para obter informações de arquivos salvos ou do SO
executando, e expor dados ou indisponibilizar a aplicação.


Cenário de Sucesso:

Atacante conseguir passar um comando como input do template da aplicação e ser executada no backend.




Cenário Reais

1) Captura de dados sensiveis salvos no sistema de arquivos do SO, Ex: arquivo de senha, configurações, etc
2) Remoção de estruturas da aplicação que comprometam o seu funcionamento


Como se previnir

1) Realizar sanitização e validação dos inputs do template para evitar o envio de códigos maliciosos para o backend


/nfs/homes/edjsanto/Downloads/serversidetemplateinjection.pdf

ref:

https://podalirius.net/en/articles/python-vulnerabilities-code-execution-in-jinja-templates/
https://github.com/payloadbox/ssti-payloads