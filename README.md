# AdiantiPHPVsCodeSnippets
Snippets PHP Adianti Framework para VSCode

Este repositório tem como objetivo compartilhar templates de código no padrão Adianti Framework.

Exemplo de criação de Snippets:

1 - Selecionar menu no VSCode: 

 File -> Preferences -> User Snippets
 
2 - Escolher escopo para o Snippet:
 - New Global Snippets file..
 - New Snippets file for 'NomeProjeto'... 
 
3 - Informar o nome do arquivo de Snippet.
 - o VScode irá salvar o arquivo como "nomeArquivo".code-snippets

4 - Criar os snippets
 - Criar conforme o exemplo abaixo:
 
    "Adiciona um componente TLabel ": {
		"scope": "PHP,php",
		"prefix": "newTLabel",
		"body": ["$$1 = new TLabel('$2');"],
		"description": "Adicionar TLabel"
    
 - As variáveis precedidas pelo caracter $ (sifrão), indicam parada do cursor seguindo a ordem numérica, ex.: $1, $2, $3...
 - Por ser o caracter $ o mesmo utilizado no PHP como prefixo de variável, o mesmo terá que ser repetida, ex. $$1 (onde o primeiro $ se torna um caracter do texto final e o segundo utilizado pelo snippet para posicionamento do cursor).
 
 - Caso forem repetidas, será repetido o conteúdo digitado para cada identificador, 
 por exemplo.: 
 
 "body": ["$$1 = new TLabel('$1');"], 
 o cursor irá parar na posição $1 e ao digitar o valor, este irá também adicionar o mesmo valor na segunda posição com a marcação $1.
 
Utilização de um arquivo de snippet externo:

Basta adicionar o(s) arquivo(s) de snippets no diretório de snippets do VSCode, exemplo:
User\AppData\Roaming\Code\User\snippets
