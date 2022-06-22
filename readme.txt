Lembre-se sempre antes de realizar qualquer coisa ligue o servidor local com um "npm start" dentro do terminal no arquivo server.js


Modelo de requisiçao get: 
/categoria

retorno do Get:
Toda a tabela categoria


/produto

retorno do Get:
Toda a tabela produto

/fornecedor

retorno do Get:
Toda a tabela fornecedor

/estoque

retorno do Get:
Toda a tabela estoque

/pedidos

retorno do get:
Toda a tabela pedidos


Modelo de requisiçao post:

(/cadastro_produtos)
{
   "nome": "nome do produto",
   "valor": valor do produto,
   "IDcategoria": ID da categoria,
   "IDfornecedor": ID do fornecedor,
   "link": "link"
}
retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro

(/cadastro_fornecedor)
{
   "nome": "nome do fornecedor",
   "email": "email",
   "cnpj": "cnpj 11 digitos",
   "telefone": "telefone de contato"
}

retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro

(/cadastro_estoque)
{
   "quantidade": quantidade existente,
   "IDproduto": produto referencia
}

retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro

(/cadastro_pedido)
{
   "IDpedido": numero do pedido,
   "IDestoque": id do produto no estoque,
   "valor": valor do item
}

retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro

Modelo de PUT:


(/update_produto)
{
   "nome": "novo nome",
   "valor": novo valor,
   "IDcategoria": novo ID da categoria(nao deixar vazio),
   "IDfornecedor": novo ID do fornecedor(nao deixar vazio),
   "link": "novo link"
   "id": id do produto que sera atualizado
}
retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro


(/update_quantidade) {atualiza apenas a quantidade de um item no estoque sem precisar atualizar o item junto}
{
   "quantidade": "nova quantidade",
   "id": id que sera atualizado
}
retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro

(/update_fornecedor)
{
   "nome": "novo nome",
   "email": "novo email",
   "cnpj": "novo cnpj",
   "telefone": "novo telefone",
   "link": "novo link"
   "id": id que sera atualizado
}
retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro


(/update_estoque)
{
   "quantidade": "nova quantidade",
   "IDproduto": "novo produto",
   "id": id que sera atualizado
}
retorno 
mensagem de confirmaçao de atualizaçao
ou msg de erro cm respectivo erro


Modelo de Delete:

'/delete_produto'
{
   "id": "id para delete"
}

retorno 
mensagem de confirmaçao de inserçao
ou msg de erro cm respectivo erro 

'/delete_fornecedor'
{
   "id": "id para delete"
}

retorno 
mensagem de confirmaçao de inserçao
ou msg de erro cm respectivo erro 

'/delete_estoque'
{
   "id": "id para delete"
}

retorno 
mensagem de confirmaçao de inserçao
ou msg de erro cm respectivo erro 

'/delete_pedido'
{
   "id": "id para delete"
}

retorno 
mensagem de confirmaçao de inserçao
ou msg de erro cm respectivo erro 

