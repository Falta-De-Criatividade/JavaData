# JavaData
Uma ideia de formato de um formato de arquivo que armazenado dados na mesma forma que são armazenados na memória e não em formatos de strings encapsulados em objetos com tipos predefinidos. Também mantém nomes para que podem ser associados a esses dados para mostrar algo mais intuitivo quando o arquivo é aberto em um editor.

Indentificadores de 2 bytes indicam a classe de um objeto também o tipo de variáveis primitivas (inteiros e boleanos) e strings.

Algo que chamei de dicionário é o que define as classes e o tipo de seus atributos internos como um objeto específico no documento (com um idenficador próprio) ou importado de outro lugar ou documento e talvez possa ser a combinação de outros dicionários. Ele só tem que precarregado pela classe que lê o ducumento antes dela começar a ler o resto do documento. Além disso ele também associa nomes com os atributos e com os demais indentificadores para gerar aquele indicativo visual no editor que falei antes.

Não projetei direito ainda, mas da forma que expliquei, os dados virão como apenas um grande array indenfinido de dados, sem nomes ou tipos algo que a camada extra que expliquei dá a eles. Eles apenas serão quebrados por 2 bytes que servem para identificar os tipos dos objetos e por valores nulos que delimitam strings.
