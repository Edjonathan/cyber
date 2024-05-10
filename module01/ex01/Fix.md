XML External Entity (XXE) Injection

Problema identificado

O frontend passar o conteúdo do input sem validação e o backend está com a resolução de entidades
externas está desativada.


Solução:

Para resolver é necessário realizar tratativa de input do frontend, e desabilitar a resolução de 
entidades externas no backend.

Obs: Para toda e qualquer lib utilizada é necessário estar com a versão mais atualizada e com ter 
conhecimento dos bugs atuais da lib