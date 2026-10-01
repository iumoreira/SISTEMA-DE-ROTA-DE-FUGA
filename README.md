# SISTEMA DE ROTA DE FUGA: CONTEXTUALIZAÇÃO TEMÁTICA
Em uma mina profunda, alguns operários estavam em busca de minerais raros. Todavia, devido um erro nos cálculos, os operários destruíram uma parte vital da mina que garantia a sustentação do teto fazendo com que o local desabasse. Esse programa simula um sensor que verifica possíveis rotas de fuga para garantir quais locais estão livres de escombros, onde E é o local que se encontra os feridos e S o ponto de saída, além de que caso não haja rota, equipes especializadas deverão ser acionadas para liberar o caminho.  

# INTRODUÇÃO AO SISTEMA
O programa inicialmente, solicita o nome de quem está operando o sistema para que se registre no arquivo .txt mais brevemente. Após isso, um menu com opções fica disponível ao operador com as opções:

     a) verificar o registro sismico;
     b) utilizar o sensor de escombros;
     d) produzir um arquivo situacional;

1) A ferramenta "verificar o registro sismico", serve como um verificador da atividade sismica atual. Utiliza-se o loop do... while e a função rand()%11 (uma vez que a escala Richther vai até esse patamar), conforme é gerado um numeral pseudoaleatorio;

2) A ferramenta "utilizar o sensor de escombros", serve como a função principal do programa que gera uma matriz de ordem 10 e disponibiliza as rotas seguras até o ponto de saída - representadas por '*' - ou irá informar caso não haja saída - representadas por '#';

3) A ferramenta "produzir um arquivo situacional" cria um arquivo .txt que guardará os dados obtidos.  Essa ferramenta guarda os dados no computador e são de natureza permanente para ser analisada posteriormente;

# SOBRE O SENSOR DE ESCOMBROS E ROTA DE FUGA
Fazer uma "varredura" do local do acidente utilizando o programa, é criar uma matriz de ordem 10. A localização do operários fixa em E e a localização da saída fixa em S, desse  modo, pode ser que eles possam estar ao lado da saída ou não. Caso não estejam, o programa identifica os escombros simbolizados por '#' e a passagem pelo '*'. Isso utilizou-se as seguintes mecânicas:

     a) os elementeos da matriz são geradas pseudoaleatoriamente (já dito na explicação (1)) com números de 0 até 100;
     b) utiliza-se o while para vazer todas a matriz e onde atenda a condição while(a %2 = 0), utilizar a função string de troca de caractere e substituir o numeral por um '*';
     c) caso a condição não seja atendida o while deve substituir (no caso os numeros ímpares) por '#';
     d) caso um dos números sejam divisíveis por 7, o programa deve substituir por um ' ' (espaço em branco);
