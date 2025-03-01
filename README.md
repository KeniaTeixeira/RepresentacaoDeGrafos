# Implementação N.01 - Representação de Grafos

## Descrição
Este projeto implementa uma representação de grafos direcionados utilizando listas de adjacência. O código foi desenvolvido como parte da disciplina de **Teoria de Grafos e Computabilidade**. O programa permite a leitura de grafos a partir de um arquivo, onde são especificados os vértices e as arestas. Em seguida, o programa fornece informações detalhadas sobre um vértice específico, como:
- Grau de saída
- Grau de entrada
- Conjunto de sucessores
- Conjunto de predecessores

### Funcionalidades:
1. **Leitura de Grafos a partir de um Arquivo**: O programa recebe um arquivo de texto que descreve o grafo, onde a primeira linha contém o número de vértices e arestas, e as linhas seguintes descrevem as arestas.
2. **Exibição de Informações do Vértice**: O usuário pode consultar informações sobre um vértice específico do grafo, como o grau de entrada, grau de saída, sucessores e predecessores.

## Formato do Arquivo de Entrada
O arquivo de entrada deve estar no seguinte formato:
1. A primeira linha contém dois números inteiros: o número de vértices e o número de arestas.
2. As linhas seguintes contêm duas colunas inteiras, representando uma aresta direcionada do vértice de origem para o vértice de destino.

### Passo 2: Executar o Programa
1. Compile e execute o programa.
2. O programa pedirá que você insira o nome do arquivo contendo o grafo.
3. Em seguida, será solicitado que você insira o número do vértice para o qual deseja visualizar as informações.
4. O programa irá exibir as informações sobre o vértice solicitado.

## Estrutura do Código
### Classe `Grafo`
- **Construtor**: Recebe o número de vértices e inicializa as estruturas de dados (lista de adjacência e grau de entrada).
- **Método `adicionarAresta`**: Adiciona uma aresta direcionada ao grafo.
- **Método `exibirInformacoesVertice`**: Exibe as informações sobre o vértice, incluindo grau de entrada, grau de saída, sucessores e predecessores.
- **Método `convertParaBase1`**: Converte a indexação interna do grafo (base 0) para uma indexação mais intuitiva (base 1).
- **Método `formatarLista`**: Formata a lista de sucessores e predecessores para exibição, removendo colchetes e vírgulas.

## Exceções Tratadas
- **Erro de Arquivo**: Caso o arquivo não possa ser lido corretamente, o programa exibe uma mensagem de erro informando o problema.
- **Entrada Inválida**: Se o usuário inserir um valor inválido para o vértice, o programa informa o erro e não trava.
