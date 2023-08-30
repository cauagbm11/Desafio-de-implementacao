CENTRO UNIVERSITÁRIO DO PARÁ - CESUPA
ESCOLA DE NEGÓCIOS, TECNOLOGIA E INOVAÇÃO - ARGO
CURSO DE ENGENHARIA DA COMPUTAÇÃO



 


ANDREY SOUZA RANIERI
CAUÃ GUERREIRO BRITTO MENDES
CÁSSIO LIMA CAVALCANTE
DOUGLAS GOBITSCH DE ALMEIDA MELLO
HENRIQUE CABRAL VELLOSO DA SILVA






						
PROJETO PRÁTICO
PROF. ISAAC ELGRABLY






BELÉM-PA
2023


1.DESCRIÇÃO DETALHADA DA ESTRUTURA DE DADOS

A função importData é responsável por importar os dados dos produtos a partir de um arquivo. Ela recebe como parâmetros um vetor de produtos e o nome do arquivo a ser importado. A função abre o arquivo, lê cada linha até atingir o limite de 100 dados ou o final do arquivo, e extrai os campos separados por espaço ou tabulação. Os valores são convertidos para os tipos adequados e um novo objeto Product é criado e adicionado ao vetor de produtos.

A função addProduct permite ao usuário adicionar um novo produto. Ela solicita ao usuário que digite o nome, descrição, preço e quantidade do produto e cria um novo objeto Product com os valores fornecidos. Em seguida, o produto é adicionado ao vetor de produtos.

A função removeProduct permite ao usuário remover um produto do vetor de produtos. Ela recebe como parâmetro o nome do produto a ser removido. Utilizando a função find_if da biblioteca <algorithm>, a função realiza uma busca no vetor de produtos para encontrar o produto com o nome correspondente. Se o produto é encontrado, ele é removido do vetor.

A função updateProduct permite ao usuário atualizar as informações de um produto existente. O usuário informa o nome do produto a ser atualizado e a função realiza uma busca no vetor de produtos para encontrar o produto correspondente. Se o produto é encontrado, o usuário pode digitar os novos valores para o nome, descrição, preço e quantidade. As informações do produto são atualizadas no vetor.

A função searchProduct permite ao usuário buscar um produto pelo nome utilizando o algoritmo de busca binária. A função recebe como parâmetros o vetor de produtos e o nome do produto a ser buscado. Utilizando a função lower_bound da biblioteca <algorithm>, a função realiza a busca binária no vetor, encontrando o primeiro produto cujo nome é maior ou igual ao nome fornecido. Se o produto é encontrado, suas informações são exibidas na tela.

As funções displayProductsByPrice e displayProductsByName permitem ao usuário visualizar os produtos em ordem crescente ou decrescente de preço e em ordem alfabética crescente ou decrescente por nome, respectivamente. Elas criam cópias do vetor de produtos e utilizam os algoritmos de ordenação Heapsort e sort da biblioteca <algorithm> para ordenar os produtos conforme o critério desejado. Em seguida, os produtos ordenados são exibidos na tela.

No main, o código inicializa um vetor de produtos, realiza a importação dos dados iniciais a partir do arquivo "produtos.txt" utilizando a função importData, e exibe um menu para o usuário poder interagir com o sistema. O usuário pode escolher entre diversas opções, como adicionar, remover, atualizar e buscar produtos, além de exibir os produtos ordenados de diferentes formas. O programa continua a executar até que o usuário escolha a opção de sair (0).


Em resumo, o código apresenta uma implementação funcional de um sistema de gerenciamento de produtos, onde as operações de adição, remoção, atualização e busca são realizadas eficientemente utilizando estruturas de dados adequadas e algoritmos de busca e ordenação eficientes. O menu fornece uma interface intuitiva para o usuário interagir com o sistema e realizar as operações desejadas.
