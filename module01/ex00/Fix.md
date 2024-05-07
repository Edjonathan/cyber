Template Injection

Problema identificado

O frontend passar o conteúdo do input template para o backend sem validação ou sanitização,
esse comportamento permite o envio de codigo malicioso para o motor de template jinja executar.
No caso do exercicio conseguimos abrir um arquivo de password com informações sensiveis e obter
as senhas contidas nele.


Solução:

A solução proposta para resolver esse cenário seria a sanitização do campo input no index.html 
para que o código malicioso não fosse enviado e executado no backend. Poderiamos ter uma validação
adicional no backend ou adição de trava de token para que não seja possivel chamar o backend diretamente
passando o codigo maliciosos