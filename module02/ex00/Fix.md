Deserialization Vunerability

Problema identificado

A aplicação recebe conteúdo no input e não realiza validação. Alem disso está utilizando a lib pickle no
python que não oferece uma deserialização segura.

Solução:

Para resolver é necessário realizar validações no input, trocar o formato de conversão para json ou trocar
a lib para outra que ofereça uma deserialização segura. 

