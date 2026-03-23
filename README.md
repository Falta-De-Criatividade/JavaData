# JavaData
Alguém vai ler isso e achar estranho ou engraçado alguém so postar a ideia sem adicionar nada ou explicar direito o motivo do repositório. Meu objetivo era poder manipular dados em um arquivo de forma mais performática e que fosse fácil de utilizar a biblioteca voltada para isso (com esse ultimo sendo mais porque não sabia utilizar JAXP). Fiz esse repositório sem nada apenas para anotar as minhas ideias pos tava sofrendo ameaças de alguém de simplesmente roubar a ideia, então tornei ela logo pública.

Uma ideia de formato de um formato de arquivo que armazenado dados na mesma forma que são armazenados na memória e não em formatos de strings encapsulados em objetos com tipos predefinidos. Também mantém nomes para que podem ser associados a esses dados para mostrar algo mais intuitivo quando o arquivo é aberto em um editor.

Indentificadores de 2 bytes indicam a classe de um objeto e também o tipo de variáveis primitivas (inteiros e boleanos) e strings mas esse dois últimos tendo IDs já predefinidos pelo algoritmo.

Algo que chamei de dicionário é o que define as classes e o tipo de seus atributos internos como um objeto específico no documento (com um idenficador próprio) ou importado de outro lugar ou documento e talvez possa ser a combinação de outros dicionários. Ele só tem que precarregado pela classe que lê o ducumento antes dela começar a ler o resto do documento. Além disso ele também associa nomes com os atributos e com os demais indentificadores para gerar aquele indicativo visual no editor que falei antes.

Não projetei direito ainda, mas da forma que expliquei, os dados virão como apenas um grande array indenfinido de dados, sem nomes ou tipos algo que a camada extra que expliquei dá a eles. Eles apenas serão quebrados por 2 bytes que servem para identificar os tipos dos objetos e por valores nulos que delimitam strings.

Também pensei em objetos parecidos com lambdas que indicam chamadas de metodos um atrás do outro e na hora de converter essa lambada, seria algo tipo um stream. Um método sendo um objeto como qualquer outro indicado pelo dicionário mas ao invés de atributos sejam guardados os parâmetros.
Não pensei o que seria necessário para diferencialos dos objetos e normais, mas talvez possa ser uma ideia util para alguém.
