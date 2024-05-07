Cross Site Request Forgery (CSRF)

Problema identificado

O Site não tem requisitos de autenticação e autorização, não trabalha com validação de token no backend.
Expõe a URL que está chamando para realizar o débito na conta do cliente e como está chamando. 
Deste modo, o atacante consegue chamar a URL do backend fora do site e realizar o debito na conta do cliente


Solução:

1) Remover a exposição de URL do frontend, isso pode ser feito adicionando um proxy reverso que conhece as URLs
2) Utilização de conexão segura de ponta a ponta.
3) Adicionar autenticação via OpenID no frontend e validação de token no backend 