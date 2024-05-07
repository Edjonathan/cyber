
Cross Site Scripting (XSS)


Descrição

É um ataque que explora vulnerabilidades através da execução de script com código malicioso no browser. Como será
executado em um browser o script precisa ser escrito em código compativel com client side, Javascript, HTML, Flash ou
qualquer outro tipo de código que executa no browser.



Cenário de Sucesso:

Um ataque tem sucesso quando um atacante consegue inserir e executar um código malicioso em um browser. 



Existem três categorias de ataques XSS: Reflected, Stored e DOM-Based Attacks


	Reflected Attack

		Quando o script malicioso bem do request HTTP atual. Esse ataque é tambem conhecido como NON-Persistent ou Type-I XSS.


	Stored Attack

		Quando o script malicioso foi gravado na base de dados da aplicação e é acionado a cada chamada realizada no site.


	DOM-Based

		Quando a vulnerabilidade existe no cliente ao invés do servidor.



Cenário Reais

1) Exposição de dados sensiveis de usuário em formulários.
2) Alteração de conteúdos importantes para gerar caos no mercado.


Como se previnir

Podemos utilizar as recomendações da OWASP para orientar os desenvolvedores com boas práticas e estabelecer um processo de
code review orientado a essas recomendações:

https://cheatsheetseries.owasp.org/cheatsheets/Cross_Site_Scripting_Prevention_Cheat_Sheet.html
