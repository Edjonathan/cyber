Server-Side Request Forgery e Local File Injection

Problema identificado

O valor de entrada do path não é validado na aplicação o que permite que retorne as informações do arquivo.
Alem disso, é retornada uma URL que permite que a exploração do SSRF


Solução:

Para resolver é necessário realizar validação e sanitização do input path informado, trabalhar com whitelist 
para demilitar as urls que podem se comunicar com aplicação e trabalhar com acesso minimo da aplicação,
para que, em caso de sucesso, o atacante não consiga realizar ações abruptas no servidor. 