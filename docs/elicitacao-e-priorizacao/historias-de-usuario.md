# Histórias de Usuário

## Introdução 

<p style="text-align: justify; text-indent: 2em;"> As histórias de usuário são uma forma de documentar requisitos de software de maneira concisa e acessível, representando as necessidades do usuário de forma clara e orientada por objetivos. Em vez de descrever funcionalidades tecnicamente, elas são narrativas curtas que enfatizam <b>quem</b> usará a funcionalidade, <b>o que</b> precisa ser feito e <b>por que</b> isso é importante. </p>

<p style="text-align: justify; text-indent: 2em;"> Essa abordagem permite capturar as intenções e expectativas dos usuários finais, facilitando a comunicação entre desenvolvedores, analistas e partes interessadas. Uma história de usuário bem definida segue o formato: </p>  

<div style="text-align: center;">
    <p><strong>Como</strong> <code>tipo de usuário</code> <strong>eu quero</strong> <code>ação ou funcionalidade</code><strong>para</strong> <code>objetivo ou valor esperado.</code></p>
</div>

<p style="text-align: justify; text-indent: 2em;"> Além disso, cada história de usuário é complementada por critérios de aceitação, que descrevem as condições mínimas para que a funcionalidade seja considerada pronta. Esses critérios servem como uma referência para validação e ajudam a evitar ambiguidades durante o desenvolvimento. </p>

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
|US01|Eu, como usuário, quero me cadastrar no sistema, para poder realizar avaliações de restaurantes.|1. O sistema deve permitir o cadastro de usuário com os seguintes dados: nome, email, senha, data de nascimento e endereço.</br>2. O sistema deve validar o formato do email.</br>3. A senha deve ter no mínimo 6 caracteres e ser confirmada.</br>4. Após o cadastro, o sistema deve enviar um email de confirmação para o endereço informado.|
|US02|Eu, como usuário autenticado, quero editar os dados da minha conta, para manter minhas informações corretas e atualizadas.|1. O sistema deve permitir que o usuário edite os dados: nome, email, senha e endereço.</br>2. O sistema deve exigir a senha atual para permitir a alteração dos dados.</br>3. O sistema deve validar os novos dados antes de confirmar a edição (exemplo: verificar se o email está em formato correto).|
|US03|Eu, como usuário autenticado, quero visualizar meu dados cadastrais, para que eu possa verificar e confirmar as informações da minha conta.|1. O sistema deve permitir a exclusão da conta do usuário.</br>2. O sistema deve pedir uma confirmação de exclusão para evitar exclusões acidentais.</br>3. Após a exclusão, todos os dados relacionados ao usuário devem ser removidos do sistema.</br>4. O usuário não deve conseguir acessar o sistema após a exclusão.|
|US04|Eu, como usuário autenticado, quero excluir minha conta, para que eu possa remover todos os dados associados a ela do sistema.|1. O sistema deve permitir o cadastro de um novo restaurante com os seguintes dados: nome, endereço, telefone, categoria, e descrição.</br>2. O sistema deve verificar se o restaurante já está cadastrado antes de permitir o cadastro.|
|US05|Eu, como usuário autenticado, quero cadastrar um restaurante, caso ele não exista ainda no sistema, para realizar uma avaliação do mesmo.||
|US06|Eu, como usuário autenticado, quero editar os dados do restaurante, para que as informações estejam atualizadas.||
|US07|Eu, como usuário, quero visualizar as informações de um restaurante, para que eu possa escolher em qual restaurante irei.||
|US08|Eu, como usuário, quero fazer login no sistema, para que eu possa acessar minha conta e realizar avaliações de restaurantes. ||
|US09|Eu, como usuário, quero fazer logout do sistema, para que minha sessão seja encerrada e minha conta fique segura até o próximo login.||
|US10|Eu, como usuário autenticado, quero realizar uma avaliação de um restaurante, para compartilhar minhas experiências.||
|US11|Eu, como usuário autenticado, quero excluir uma avaliação que fiz anteriormente, para que minha opinião seja removida.||
|US12|Eu, como usuário, quero filtrar restaurantes por categorias, para encontrar mais facilmente os restaurantes que podem me interessar.||
|US13|Eu, como usuário, quero buscar por restaurantes específicos, para encontrar avaliações dos mesmos.||
|US14|Eu, como usuário, quero visualizar todas as avaliações que fiz, para revisar o que já avaliei.||
|US15|Eu, como usuário, desejo visualizar as avaliações que eu escrevi para um restaurante no topo da lista de avaliações do respectivo restaurante, para revisar o que já avaliei.||


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
| `1.1`  |27/11/2024| Adicionando histórias de usuário | [Júlia Yoshida](https://github.com/juliaryoshida) |[Maria Alice](https://github.com/Maliz30)|