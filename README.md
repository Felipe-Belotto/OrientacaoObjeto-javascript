# OrientacaoObjeto-javascript

    Esse projeto foi desenvolvido durante o Curso de Javascript Puro Orientado a Objetos 
    do canal ProgramadorEspartano, 
    todos os créditos e agradecimento pelo curso gratuito no youtube.

   [Veja o projeto pelo Vercel](https://orientacao-objeto-javascript.vercel.app/)

   Resumo do código js

   O código é uma classe chamada "Produto" que possui métodos que permitem adicionar, atualizar, deletar e listar produtos em uma tabela HTML.

O método "constructor" define três variáveis, "id", "arrayProdutos" e "editId". O método "salvar" verifica se os campos do produto são válidos e, em seguida, adiciona o produto ao array de produtos ou atualiza o produto existente se o editId não for nulo. Depois, chama o método "listaTabela" e "cancelar".

O método "listaTabela" busca o elemento tbody na tabela HTML, limpa seu conteúdo e adiciona uma linha para cada produto no array de produtos. Cada linha contém células para o ID do produto, nome, preço e botões de edição e exclusão.

O método "adicionar" recebe um objeto de produto e adiciona ao array de produtos. Também atualiza a variável "id".

O método "atualizar" recebe um ID de produto e um objeto de produto, percorre o array de produtos procurando um produto com o ID correspondente e atualiza as informações do produto.

O método "preparaEdicao" recebe um objeto de produto e atualiza os campos de entrada HTML com as informações do produto. Também atualiza o texto do botão "Salvar" para "Atualizar" e atualiza o valor de "editId".

O método "lerDados" lê as informações do produto a partir dos campos de entrada HTML e retorna um objeto de produto com as informações.

O método "validaCampos" recebe um objeto de produto e verifica se os campos obrigatórios são preenchidos. Se houver campos em branco, exibe uma mensagem de alerta e retorna falso. Caso contrário, retorna verdadeiro.

O método "cancelar" limpa os campos de entrada HTML e atualiza o texto do botão "Salvar" para "Salvar". Também define "editId" como nulo.

O método "deletar" recebe um ID de produto e verifica se o usuário deseja realmente excluir o produto. Se o usuário confirmar, percorre o array de produtos procurando um produto com o ID correspondente e remove-o do array de produtos e da tabela HTML.