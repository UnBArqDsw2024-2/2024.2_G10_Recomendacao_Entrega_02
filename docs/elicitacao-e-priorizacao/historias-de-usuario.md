# Histórias de Usuário

## Introdução 

<p style="text-align: justify; text-indent: 2em;"> As histórias de usuário são uma forma de documentar requisitos de software de maneira concisa e acessível, representando as necessidades do usuário de forma clara e orientada por objetivos. Em vez de descrever funcionalidades tecnicamente, elas são narrativas curtas que enfatizam <b>quem</b> usará a funcionalidade, <b>o que</b> precisa ser feito e <b>por que</b> isso é importante. </p>

<p style="text-align: justify; text-indent: 2em;"> Essa abordagem permite capturar as intenções e expectativas dos usuários finais, facilitando a comunicação entre desenvolvedores, analistas e partes interessadas. Uma história de usuário bem definida segue o formato: </p>  

<div style="text-align: center;">
    <p><strong>Como</strong> <code>tipo de usuário</code> <strong>eu quero</strong> <code>ação ou funcionalidade</code><strong>para</strong> <code>objetivo ou valor esperado.</code></p>
</div>

<p style="text-align: justify; text-indent: 2em;"> Além disso, cada história de usuário é complementada por critérios de aceitação, que descrevem as condições mínimas para que a funcionalidade seja considerada pronta. Esses critérios servem como uma referência para validação e ajudam a evitar ambiguidades durante o desenvolvimento. </p>


## Tipos de usuário

<p style="text-align: justify; text-indent: 2em;">O sistema foi projetado para atender a diferentes tipos de usuários que interagem com a plataforma. Cada tipo de usuário possui necessidades específicas e desempenha funções distintas no sistema. Basicamente, temos dois tipos de usuários: </p>

1. Usuário Visitante
   - Descrição: Pessoas que acessam o sistema pela primeira vez ou sem realizar login.
   - Necessidades:
      - Visualizar informações públicas sobre restaurantes.
      - Buscar e filtrar restaurantes por categorias.
   - Objetivo: Explorar informações e decidir se deseja se cadastrar para usufruir de funcionalidades mais avançadas.

2. Usuário cadastrado
   - Descrição: Pessoas cadastradas que realizam login no sistema.
   - Necessidades:
      - Avaliar restaurantes com notas e comentários.
      - Gerenciar suas informações pessoais (editar ou excluir).
      - Cadastrar novos restaurantes no sistema.
      - Editar ou excluir avaliações realizadas anteriormente.
   - Objetivo: Compartilhar suas experiências gastronômicas e acessar funcionalidades personalizadas.   


## Metodologia 

<p style="text-align: justify; text-indent: 2em;"> A representação das histórias de usuário seguirá o seguinte padrão: </p>


<div align="center">

   <font size="3">
         <p><b>Tabela 1:</b> Estrutura da Tabela</p>
   </font>

|Identificador|História de usuário|Critérios de aceitação|
|--|--|--|
| - | - | - |

   <font size="3">
         <p><b>Fonte:</b> <a href="https://github.com/juliaryoshida">Júlia Yoshida</a>, 2024</p>
   </font>

</div>

<p style="text-align: justify; text-indent: 2em;">Onde:</p>

 - **Identificador**: Um código único atribuído à história de usuário para identificá-lo de forma clara e inequívoca dentro do projeto. Facilita o rastreamento e a referência durante o desenvolvimento, testes e manutenção. Exemplo: US01(User Story 01).
 - **História de usuário**: Um rótulo curto e direto que identifica o requisito de forma resumida.
 - **Critérios de aceitação**: Os critérios de aceitação funcionam como um conjunto de regras e testes que devem ser atendidos para garantir que o sistema esteja funcionando conforme esperado. Eles servem como uma base para validar a entrega da funcionalidade e garantir que o resultado esteja alinhado com os requisitos do usuário.

## Histórias de Usuário

<div align="center">
   <font size="3">
         <p><b>Tabela 2:</b> Histórias de usuário</p>
   </font>

|Identificador|História de Usuário|Critérios de aceitação|
|-|-|-|
|US01|Eu, como usuário visitante, quero me cadastrar no sistema, para poder realizar avaliações de restaurantes.|1. O sistema deve permitir o cadastro de usuário com os seguintes dados: nome, email, senha, data de nascimento e endereço.</br>2. O sistema deve validar o formato do email.</br>3. A senha deve ter no mínimo 6 caracteres e ser confirmada.</br>4. Após o cadastro, o sistema deve enviar um email de confirmação para o endereço informado.|
|US02|Eu, como usuário cadastrado, quero editar os dados da minha conta, para manter minhas informações corretas e atualizadas.|1. O sistema deve permitir que o usuário edite os dados: nome, email, senha e endereço.</br>2. O sistema deve exigir a senha atual para permitir a alteração dos dados.</br>3. O sistema deve validar os novos dados antes de confirmar a edição (exemplo: verificar se o email está em formato correto).|
|US03|Eu, como usuário cadastrado, quero visualizar meu dados cadastrais, para que eu possa verificar e confirmar as informações da minha conta.|1. O sistema deve exibir todos os dados cadastrados pelo usuário de forma clara.</br>2. Os dados devem ser apresentados de forma somente leitura (não editáveis).</br>3. O usuário pode acessar a visualização dos dados a qualquer momento em sua conta.|
|US04|Eu, como usuário cadastrado, quero excluir minha conta, para que eu possa remover todos os dados associados a ela do sistema.|1. O sistema deve permitir a exclusão da conta do usuário.</br>2. O sistema deve pedir uma confirmação de exclusão para evitar exclusões acidentais.</br>3. Após a exclusão, todos os dados relacionados ao usuário devem ser removidos do sistema.</br>4. O usuário não deve conseguir acessar o sistema após a exclusão.|
|US05|Eu, como usuário cadastrado, quero cadastrar um restaurante, caso ele não exista ainda no sistema, para realizar uma avaliação do mesmo.|1. O sistema deve permitir o cadastro de um novo restaurante com os seguintes dados: nome, endereço, telefone e categoria.</br>2. O sistema deve verificar se o restaurante já está cadastrado antes de permitir o cadastro.|
|US06|Eu, como usuário cadastrado, quero editar os dados do restaurante, para que as informações estejam atualizadas.|	1. O sistema deve permitir a edição dos dados do restaurante: nome, endereço, telefone e categoria.</br>2. O sistema deve exigir autenticação para que o usuário consiga editar os dados.</br>3. O sistema deve garantir que as edições não resultem em dados inválidos (exemplo: verificar se o telefone tem o formato correto).|
|US07|Eu, como usuário visitante/usuário cadastrado, quero visualizar as informações de um restaurante, para que eu possa escolher em qual restaurante irei.|1. O sistema deve exibir as informações do restaurante: nome, endereço e telefone, e categoria.</br>2. O sistema deve também mostrar as avaliações de outros usuários sobre o restaurante.</br>3. A visualização deve ser clara e fácil de entender.|
|US08| Eu, como usuário usuário cadastrado, quero excluir um restaurante, para remover-lo do sistema caso ele deixe de existir | 1. O sistema deve permitir a exclusão do restaurante. <br>2. O sistema deve pedir uma confirmação de exclusão para evitar exclusões acidentais. <br>3. Após a exclusão, todos os dados relacionados ao restaurante excluído devem ser removidos do sistema. |
|US09|Eu, como usuário cadastrado, quero fazer login no sistema, para que eu possa acessar minha conta e realizar avaliações de restaurantes. |1. O sistema deve permitir login com email e senha.</br>2. O sistema deve validar as credenciais e permitir o acesso somente se os dados estiverem corretos.</br>3. Se o login for bem-sucedido, o usuário será redirecionado para a página principal ou seu perfil.|
|US10|Eu, como usuário cadastrado, quero fazer logout do sistema, para que minha sessão seja encerrada e minha conta fique segura até o próximo login.|1. O sistema deve permitir que o usuário faça logout clicando em um botão de "Logout".</br>2. Após o logout, o usuário não poderá acessar suas informações sem realizar novo login.</br>3. O sistema deve redirecionar para a página inicial ou de login após o logout.|
|US11|Eu, como usuário cadastrado, quero realizar uma avaliação de um restaurante, para compartilhar minhas experiências.|1. O sistema deve permitir a avaliação com uma nota (de 1 a 5) e um comentário opcional.</br>2. A avaliação deve ser vinculada ao restaurante selecionado.</br>3. O sistema deve exigir que o usuário esteja logado para realizar a avaliação.|
|US12|Eu, como usuário cadastrado, quero excluir uma avaliação que fiz anteriormente, para que minha opinião seja removida.|1. O sistema deve permitir a exclusão de avaliações feitas pelo usuário.</br>2. O sistema deve pedir confirmação antes de excluir a avaliação.</br>3. Após a exclusão, a avaliação não deve mais aparecer nas listagens do restaurante.|
|US13|Eu, como usuário visitante/usuário cadastrado, quero filtrar restaurantes por categorias, para encontrar mais facilmente os restaurantes que podem me interessar.|1. O sistema deve permitir filtrar restaurantes pelas seguintes categorias:</br>- Brasileira;</br>- Japonesa;</br>- Chinesa;</br>- Italiana;</br>- Árabe;</br>- Doces e sobremesas;</br>- Mexicana;</br>- Fast-food;</br>- Padaria/Café;</br>- Hambúrguer;</br>- Lámen;</br>- Pizza;</br>- Bolos;</br>- Sorvete;</br>- Café da manhã;</br>- Vegano;</br>- Sem glúten;</br>- Vegetariano;</br>- Bebidas;</br>- Self-service;</br>- Churrasco;</br>- Frutos do mar.</br>2. O sistema deve exibir somente os restaurantes que correspondem à categoria selecionada.|
|US14|Eu, como usuário visitante/usuário cadastrado, quero buscar por restaurantes específicos, para encontrar avaliações dos mesmos.|1. O sistema deve permitir a busca por nome de um restaurante.</br>2. O sistema deve exibir resultados relevantes baseados na busca realizada.|
|US15|Eu, como usuário cadastrado, quero visualizar todas as avaliações que fiz, para revisar o que já avaliei.|1. O sistema deve exibir todas as avaliações feitas pelo usuário em uma página específica do perfil.</br>2. As avaliações devem ser listadas com os detalhes de cada restaurante e a nota atribuída.|
|US16|Eu, como usuário cadastrado, desejo visualizar as avaliações que eu escrevi para um restaurante no topo da lista de avaliações do respectivo restaurante, para revisar o que já avaliei.|1. O sistema deve exibir as avaliações do usuário no topo da lista de avaliações do restaurante.</br>2. O sistema deve identificar e destacar as avaliações feitas pelo usuário.|
|US17| Eu, como usuário visitante, quero visualizar todas as avaliações já cadastradas para um restaurante |1. O sistema deve exibir uma listagem de todas as avaliações realizadas para um restaurante, contendo: nome do usuário que cadastrou a avaliação, nota e comentário. |
|US18| Eu, como usuário cadastrado, quero curtir uma avaliação cadastrada para sinalizar que concordo com a informação que nela foi escrita |1. O sistema deve permitir que o usuário faça uma curtida por comentário. <br> 2. Caso o comentário já esteja curtido, deve ser exibida a opção de remover curtida no lugar da opção de curtir comentário.|
|US19| Eu, como usuário visitante/usuário cadastrado, quero alternar a ordenação das avaliações de acordo com a data de criação ou número de curtidas, para facilitar minha análise e escolha por um restaurante |1. O sistema deve exibir duas opções de ordenação, ordenar por data de criação e ordenar por número de curtidas.|



   <font size="3">
         <p><b>Fonte:</b> <a href="https://github.com/juliaryoshida">Júlia Yoshida</a>, 2024</p>
   </font>
</div>

## Bibliografia

## Referências Bibliográficas

> **PRESSMAN, Roger S**. Engenharia de software: uma abordagem profissional. 8. ed. Porto Alegre: McGraw-Hill, 2016.
>
> **COHN, Mike**. User stories applied: for agile software development. Boston: Addison-Wesley, 2004.
>
> **PATTON, Jeff**. User Story Mapping: Discover the Whole Story, Build the Right Product. 1. ed. Sebastopol: O'Reilly Media, 2014.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |19/11/2024| Adicionando introdução e metodologia das US | [Júlia Yoshida](https://github.com/juliaryoshida) |[Maria Alice](https://github.com/Maliz30)|
| `1.1`  |27/11/2024| Adicionando histórias de usuário | [Júlia Yoshida](https://github.com/juliaryoshida) |[Guilherme Brito](https://github.com/GuilhermeB12)|
| `1.2`  |27/11/2024| Adicionando tipos de usuário | [Júlia Yoshida](https://github.com/juliaryoshida) |[Caio Mesquita](https://github.com/Caiomesvie)|
| `1.3`  |28/11/2024| Adicionando histórias de usuário | [Maria Alice](https://github.com/Maliz30) | [Júlia Yoshida](https://github.com/juliaryoshida) |