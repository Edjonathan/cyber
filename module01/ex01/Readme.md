XML External Entity (XXE) Injection


Descrição

É um ataque que explora vulnerabilidades em XML Parser da aplicação. Um XML é enviado para a aplicaçao contendo uma instrução
para uma entidade externa que permite o atancante rodar comandos no SO para obtenção de dados sensiveis ou execução de comandos
que pode comprometer a infra da aplicação.

Quando não há validação, sanitização e tratativas adequadas no XML e o parser não estiver com as suas validações de processamento
de entidades externas ativadas, a aplicação está em risco. Ex: Usuário pode passar comandos para obter informações de arquivos salvos ou do SO
executando, e expor dados ou indisponibilizar a aplicação.


Cenário de Sucesso:

Atacante conseguir passar um comandos via XML para o SO e conseguir executar com sucesso a ação.



Cenário Reais

1) Captura de dados sensiveis salvos no sistema de arquivos do SO, Ex: arquivo de senha, configurações, etc
2) Remoção de estruturas da aplicação que comprometam o seu funcionamento


Como se previnir

1) Desabilitar o suporte a entidades externas
2) Ativar validação da segurança da lib de parser utilizada