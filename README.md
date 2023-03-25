# Super-market

Descrição do projeto!
Conforme solicitado, ultilizado o CRUD e o API REST.

Tecnologias ultilizadas:
Postman (para testes)
API REST
Intellij IDE 
DBeaver (Banco de dados)

Como cadastrar um produto:
No Intellij IDE, abra o projeto, roda a aplicação em seguida ultilize a url:         no Postiman apontar a url para POST para criar um produto.
Após criar o produto, clicar no Body e colocar a informação, ("Cadastro de produtos").
click em "RAW" e troque o tipo de texto para JSON.
Clicar em SEND para criar o produto e suas caracteristicas.
Tenha certeza que foi criado, mudando mudando o POST para GET, logo os produtos serão trazidos.
DELETE: Para deletar o bairro cadastrado por ID(identificador), basta trocar o GET por DELET e na barra da url acrescentar o "barra com o ID" vejamos o exemplos:
 http://localhost:8080/produto/3, Aqui está o exemplo de como deletar o bairro por ID , verifique se o ID está correto e dê um send , ele irá retornar True
ou false , se for true é pq ele deletou corretamente , se for false é porque não tem o ID correspondente.

#Como cadastrar uma categoria
Para cadastrar uma categoria segue a mesma lógica do produto, basta trocar a url, vejamos: http://localhost:8080/produto 
Após isso no Body cole essa informação:  IMPORTANTE LEMBRAR QUE NO BODY TROQUE "NONE" POR RAW E TROQUE O TIPO DE TEXT PARA JSON

{
    "nomeProduto": "Produto",
    "Comprado": "produto comprado",
    "status": "Comprado"
}
Vá em send para gerar o produto e de um get para ver se cadastrou .
Agora para cadastrar uma categoria no produto, assim que colar na url, a categoria sera cadastrada um produto e para funcionar é nececssario colocar o ID do produto no BODY. 

{
    "nomeProduto": "produto",
     "comprado":{
        "id":3
    },
    "comprado": "produto comprado",
    "status": "comprado"
}
Não sera possivel Deletar um produto com a categoria cadastrada . (Conforme solicitação)

#Listagem de produtos comprados

Para listar os produtos comprados coloque na url :    http://localhost:8080/produtos/cadastrados 
Mude para GET , para puchar os produtos cadastrados.







