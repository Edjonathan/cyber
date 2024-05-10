Deserialization Vunerability

Descrição

É um ataque que explora vulnerabilidades no processo de desserialização nativo das linguagens. Quando não ha validação nos inputs da
aplicação e utilização de libs que não seguras o atancante consegue executar códigos remotamente na aplicação.


Cenário de Sucesso:

Atacante conseguir passar um comandos via input e forçar a execução da deserialização da aplicação com sucesso.



Cenário Reais

1) Captura de dados sensiveis salvos no sistema de arquivos do SO, Ex: arquivo de senha, configurações, etc
2) Remoção de estruturas da aplicação que comprometam o seu funcionamento


Como se previnir

1) Utilizar libs e formatos(json) seguros
2) Realizar validação nos inputs da aplicação

Ref:

https://rodolfomarianocy.medium.com/insecure-deserialization-entenda-e-explore-f9c31bba85a2
