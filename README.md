App de simulação de um e-commerce de produtos naturais.

Linguagem utilizada: Kotlin

🔨 Funcionalidades do projeto
O projeto permite acessar a tela de login, cadastro, autenticação de usuário, e também, sair do App caso esteja autenticado. Além disso, possibilita a criação de produto e listagem dos produtos de cada usuário. Além disso, mantém os comportamentos de editar e remover produtos.
￼


✔️ Técnicas e tecnologias utilizadas
* Fluxo de autenticação com DataStore: armazenar tipos primitivos via preferences, como por exemplo, o id do usuário autenticado
* Migration: permitir que o App evolua cada vez que as entidades do Room são modificadas, pois modificam também o schema do banco de dados
* Coroutines e Flow: utilizados para fazer a comunicação com o Room e o DataStore
* StateFlow: permitir a alteração do valor do Flow fora do builder, como por exemplo, atualizar o valor ao coletar novos valores de um outro Flow.
* Activity base: compartilhar código comum entre as Activities, como por exemplo, código de autenticação que permite acessar o usuário logado, deslogar do App e verificar se o usuário está ou não logado
* Relacionamento no Room: configurar entidade para identificar a qual registro ela pertence, como por exemplo, um produto que pertence a um usuário.


