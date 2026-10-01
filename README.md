# SISTEMA DE ROTA DE FUGA: CONTEXTUALIZAÇÃO TEMÁTICA
Em uma mina profunda, alguns operários estavam em busca de minerais raros. Todavia, devido um erro nos cálculos, os operários destruíram uma parte vital da mina que garantia a sustentação do teto fazendo com que o local desabasse. Esse programa simula um sensor que verifica possíveis rotas de fuga para garantir quais locais estão livres de escombros, onde E é o local que se encontra os feridos e S o ponto de saída, além de que caso não haja rota, equipes especializadas deverão ser acionadas para liberar o caminho.  

# INTRODUÇÃO AO SISTEMA
O programa inicialmente, solicita o nome de quem está operando o sistema para que se registre no arquivo .txt mais brevemente. Após isso, um menu com opções fica disponível ao operador com as opções:

     a) verificar o registro sismico;
     b) utilizar o sensor de escombros;
     c) consultar os últimos registros sísmicos;
     d) produzir um arquivo situacional;

1) A ferramenta "verificar o registro sismico", serve como um verificador da atividade sismica atual. Utiliza-se o loop do... while e a função rand()%11 (uma vez que a escala Richther vai até esse patamar), conforme é gerado um numeral pseudoaleatorio;

2) A ferramenta "utilizar o sensor de escombros", serve como a função principal do programa que gera uma matriz de ordem 10 e disponibiliza as rotas seguras até o ponto de saída - representadas por '*' - ou irá informar caso não haja saída - representadas por '#';

3) A ferramenta "consultar os últimos registros sísmicos", serve um registrador dos últimos registros susmicos gerados pela ferramenta (a). Essa ferramenta é totalmente para visualização rápida de métricas estatísticas;

4) A ferramenta "produzir um arquivo situacional" cria um arquivo .txt que guardará os dados obtidos. Ao contrário da ferrammenta (c), essa ferramenta guarda os dados no computador e são de natureza permanente;
