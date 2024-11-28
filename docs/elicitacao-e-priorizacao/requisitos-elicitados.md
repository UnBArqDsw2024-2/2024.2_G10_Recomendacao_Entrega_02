# Representação dos Requisitos Funcionais

## Introdução

<p style="text-align: justify; text-indent: 2em;"> A representação dos requisitos funcionais é um passo essencial no desenvolvimento de software, uma vez que define claramente as funcionalidades e comportamentos que o sistema deve apresentar. Os requisitos funcionais são descrições detalhadas do que o sistema deve fazer, como processar dados, interagir com os usuários e outros sistemas, ou realizar tarefas específicas. Essas informações servem como base para o desenvolvimento, testes e validação do sistema.</p>

<p style="text-align: justify; text-indent: 2em;"> Representar requisitos de forma clara e precisa é fundamental para garantir que os desenvolvedores compreendam as expectativas dos stakeholders e construam o sistema de acordo com essas necessidades. Além disso, a representação adequada reduz o risco de mal-entendidos, atrasos ou falhas no projeto.</p>

<p style="text-align: justify; text-indent: 2em;"> Autores como Sommerville (2011) e Pressman (2014) destacam que a correta representação dos requisitos não só facilita a comunicação entre as partes envolvidas no projeto, mas também ajuda a identificar e corrigir problemas de maneira mais eficiente durante o ciclo de vida do desenvolvimento.</p>

## Metodologia

<p style="text-align: justify; text-indent: 2em;"> Para que pudéssemos representar e organizar os requisitos, primeiramente foi necessário identificar os stakeholders e elicitar os requisitos do sistema. Para isso, durante o Design Sprint, realizamos <a href="https://unbarqdsw2024-2.github.io/2024.2_G10_Recomendacao_Entrega_01/#/Base/1.1.DesignSprint?id=quem-s%c3%a3o-os-usu%c3%a1rios">questionários</a> para identificar os potenciais usuários do sistema e de técnicas de coleta de requisitos, como <a href="https://unbarqdsw2024-2.github.io/2024.2_G10_Recomendacao_Entrega_01/#/Base/1.1.DesignSprint?id=brainstorm">Brainstorming</a> e <a href="https://unbarqdsw2024-2.github.io/2024.2_G10_Recomendacao_Entrega_01/#/Base/1.1.DesignSprint?id=etapa-4-prototipar">Protótipos</a>. Os links das palavras destacadas levam para a sua documentação.</p>

<p style="text-align: justify; text-indent: 2em;"> A técnica escolhida para a representação de requisitos foi a descrição textual estruturada. A descrição textual estruturada é uma técnica amplamente utilizada para representar requisitos funcionais em projetos de software. Ela organiza os requisitos de forma clara e objetiva, descrevendo o que o sistema deve fazer sem ambiguidades, facilitando a comunicação entre todos os envolvidos no processo de desenvolvimento. Esse formato é frequentemente usado em projetos de pequeno e médio porte, onde os requisitos podem ser definidos com relativa simplicidade, sem a necessidade de diagramas complexos. </p>

<p style="text-align: justify; text-indent: 2em;">Portanto, decidimos por representar os requisitos funcionais elicitados da seguinte forma: </p>

<div align="center">

|Identificador|Nome|Descrição|
|--|--|--|
| - | - | - |

</div>
<p style="text-align: justify; text-indent: 2em;">Onde:</p>

 - **Identificador**: Um código único atribuído ao requisito para identificá-lo de forma clara e inequívoca dentro do projeto. Facilita o rastreamento e a referência durante o desenvolvimento, testes e manutenção. Exemplo: RF01(Requisito Funcional 01).
 - **Nome**: Um rótulo curto e direto que identifica o requisito de forma resumida.
 - **Descrição**: Uma explicação detalhada do requisito, descrevendo a funcionalidade ou característica que o sistema deve ter.


## Requisitos Funcionais

<p style="text-align: justify; text-indent: 2em;">A seguir, temos a tabela de requisitos funcionais:</p>

|Identificador|Nome|Descrição|
|--|--|--|
| RF01 | Cadastrar usuário | O sistema deve permitir que novos usuários se cadastrem informando nome completo, e-mail, senha e telefone. O sistema deve validar a unicidade do e-mail e enviar um e-mail de confirmação após o cadastro. |
| RF02 | Editar dados da conta de usuário | O sistema deve permitir que usuários autenticados editem suas informações de conta, como nome, e-mail e senha. O sistema deve validar as alterações para garantir que o e-mail seja único. |
| RF03 | Visualizar dados de conta de usuário | O sistema deve permitir que um usuário autenticado visualize seus dados cadastrais, incluindo nome, e-mail e telefone. |
| RF04 | Excluir conta de usuário | O sistema deve permitir que um usuário autenticado exclua sua conta, removendo todos os dados relacionados a ela do sistema. A exclusão deve ser permanente após a confirmação do usuário. |
| RF05 | Cadastro de restaurante | - |
| RF06 | Editar dados de restaurante | - |
| RF07 | Visualizar dados de restaurante | O sistema deve permitir que os usuários visualizem as informações de um restaurante, incluindo nome, tipo de culinária, endereço e horários de funcionamento. |
| RF08 | Excluir restaurante cadastrado | - |
| RF09 | Login de usuário | O sistema deve permitir que um usuário autenticado faça login no sistema utilizando seu e-mail e senha. O sistema deve verificar a autenticidade das credenciais e permitir o acesso ao sistema se as informações forem válidas. |
| RF10 | Logout de usuário | O sistema deve permitir que um usuário autenticado realize logout, desconectando sua sessão e garantindo que não haja mais acesso às funcionalidades restritas até o próximo login. |

## Bibliografia

> Sommerville, I. Software Engineering. Addison-Wesley, 2011.
>
> Pressman, R. S. Engenharia de Software: uma abordagem profissional. McGraw Hill, 2020.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |27/11/2024| Adicionando introdução e metodologia | [Júlia Yoshida](https://github.com/juliaryoshida) |[Maria Alice](https://github.com/Maliz30) |
| `1.1`  |27/11/2024| Adicionando requisitos| [Júlia Yoshida](https://github.com/juliaryoshida) |[Maria Alice](https://github.com/Maliz30) |