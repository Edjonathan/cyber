
Cross Site Scripting (XSS)

Cenário de Sucesso:

Um ataque tem sucesso quando um atacante consegue inserir e executar um código malicioso em um browser. 


Solução:

Garantir que todas as variaveis da interface terão validação e estejam com tratativa de escaped e sanitized

1) Aplicaria a técnica de output encoding para tratar o campo userInput de modo que ele não fosse tratado como um HTML
	1.1) Receber a variavel userInput e passá-la para a função responsavel por fazer o encoding
    	 var userInput = document.getElementById("inputText").value;
    	 var userInputSecure = decodingHTML(userInput)

    2.1) Passar essa variavel para a resposta
    	document.getElementById("output").InnerHTML = "<b>" + userInputSecure + "</b>";