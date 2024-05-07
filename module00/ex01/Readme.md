
Cross Site Request Forgery (CSRF)


Descrição

É um ataque que explora vulnerabilidades na aplicação para forçar o usuário executar ações indesejadas. O atacante tem como objetivo
utilizar técnicas para obter as informações necessárias, tais como token, parametros expostos incorretamente na URL, para realizar ações 
como se fosse o usuário logado. Exemplo: Usuário realizando uma operação de transferencia em que os dados recuperados para transação 
são expostos na URL de forma insegura. O atacante pode alterar os dados da URL e alterar para que a transferencia seja executada para ele.
Esse tipo de ataque é bem comum se o site não tiver validação de autenticação e autorização, e exposição de dados sensiveis de modo que 
fique vulneravel ao atacante.


Cenário de Sucesso:

Usuário conseguir obter informações sensiveis, alterá-las e conseguir alterar a transação para beneficio próprio.




Cenário Reais

1) Transferencia Bancaria para o atancante devido a manipulação de dados sensiveis da transação
2) Transferencia Bancaria com o token armazenado no browser


Como se previnir

1) Utilização de criptografia nos dados da requisição de ponta a ponta.
2) Utilização de validação de token no backend para validação de que trata-se de um token gerado por um processo seguro
   ex: JWT e dentro do prazo de expiração.
