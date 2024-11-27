# Diagrama de Comunicação/Colaboração

## Introdução
<p style="text-align: justify; text-indent: 2em;"> O diagrama de comunicação é um dos principais tipos de diagramas de interação definidos pela UML (Unified Modeling Language), projetado para representar a dinâmica de um sistema, destacando como os elementos se comunicam entre si durante a execução de um processo. Ele é amplamente utilizado na modelagem de sistemas para capturar as interações e trocas de mensagens entre componentes, atores e objetos que participam de um caso de uso.</p>

## Metodologia
<p style="text-align: justify; text-indent: 2em;"> O diagrama de comunicação foi realizado utilizando a plataforma Miro, para sua criação, já que utilizando esta plataforma seria possível que todos os participantes tivessem acesso e pudessem colaborar com a criação do diagrama. </p>

<p style="text-align: justify; text-indent: 2em;"> Para criar o diagrama, os participantes se reuniram para discutir e tomar as decisões sobre o mesmo. Assim foi possível estabelecer relações de comunicações e troca de mensagens entre componentes, utilizando como base o diagrama de classes previamente feito, o que tornou possível que fosse visto com mais clareza como esses processos se comunicariam.</p>

<p style="text-align: justify; text-indent: 2em;"> A seguir, se encontra a descrição dos componentes do diagrama.</p>

1. **Objetos**: Os objetos podem representar classes, entidades ou componentes do sistema que está sendo modelado.

<div align="center">
    <p style="text-align: center"><b>Figura 1:</b> Objeto que representa uma classe</p>
    <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/diagrama-de-comunicacao/docs/imagens/descricaodiagramacolaboracao1.png" alt="Objeto que representa uma classe" >
    <font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, <a href="https://github.com/juliaryoshida">Júlia Yoshida</a> e <a href="https://github.com/Maliz30">Maria Alice</a>,  2024.</p></font>
</div>

2. **Instância de um objeto**: Uma instância de objeto representa um objeto específico que interage com outros objetos no contexto de um cenário. No exemplo a seguir, temos uma instância de objeto por representarmos como "r:Avaliação", ao invés de apenas "Avaliação".

<div align="center">
    <p style="text-align: center"><b>Figura 2:</b> Objeto que representa uma classe</p>
    <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/diagrama-de-comunicacao/docs/imagens/descricaodiagramacolaboracao4.png" alt="Objeto que representa uma classe" >
    <font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, <a href="https://github.com/juliaryoshida">Júlia Yoshida</a> e <a href="https://github.com/Maliz30">Maria Alice</a>,  2024.</p></font>
</div>

3. **Links**: Os links são linhas que representam o relacionamento entre dois objetos.

<div align="center">
    <p style="text-align: center"><b>Figura 3:</b> Links</p>
    <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/diagrama-de-comunicacao/docs/imagens/descricaodiagramacolaboracao2.png" alt="Links" >
    <font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, <a href="https://github.com/juliaryoshida">Júlia Yoshida</a> e <a href="https://github.com/Maliz30">Maria Alice</a>,  2024.</p></font>
</div>

4. **Mensagens numeradas, setas e asteriscos**: As mensagens numeradas são marcadores numéricos que indicam a ordem do fluxo de interações dentro do sistema. As setas representam a direção da chamada ou resposta. Por fim, os asteriscos indicam repetições.

<div align="center">
    <p style="text-align: center"><b>Figura 4:</b> Número de sequência </p>
    <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/diagrama-de-comunicacao/docs/imagens/descricaodiagramacolaboracao3.png" alt="Número de sequência" >
    <font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, <a href="https://github.com/juliaryoshida">Júlia Yoshida</a> e <a href="https://github.com/Maliz30">Maria Alice</a>,  2024.</p></font>
</div>

5. **Mensagem condicional**: As condições são representadas entre colchetes. As condicionais são utilizadas para identificar que o método só será executado caso sejam satisfeitas. Na figura 5, temos que o fluxo será seguido caso o usuário não possua conta.

<div align="center">
    <p style="text-align: center"><b>Figura 5:</b> Condicional </p>
    <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/diagrama-de-comunicacao/docs/imagens/descricaodiagramacolaboracao5.png" alt="Condicional" >
    <font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, <a href="https://github.com/juliaryoshida">Júlia Yoshida</a> e <a href="https://github.com/Maliz30">Maria Alice</a>,  2024.</p></font>
</div>


## Diagrama de Comunicação

<p style="text-align: justify; text-indent: 2em;">O diagrama a seguir é um Diagrama de Comunicação/Colaboração UML que representa as interações entre diferentes instâncias de objetos do sistema Chef Indica, cujo objetivo principal é permitir que usuários busquem restaurantes, filtrem categorias, realizem avaliações, e façam outras operações relacionadas. Cada objeto no diagrama é uma instância específica de uma classe, e as mensagens numeradas indicam a sequência de operações realizadas no sistema.</p>

<div align="center">
    <p style="text-align: center"><b>Figura 6:</b> Diagrama de comunicação/colaboração do sistema</p>
    <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/diagrama-de-comunicacao/docs/imagens/diagramadecolaboracao.jpg" alt="Diagrama de comunicação/colaboração do sistema" >
    <font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, <a href="https://github.com/juliaryoshida">Júlia Yoshida</a> e <a href="https://github.com/Maliz30">Maria Alice</a>,  2024.</p></font>
</div>

<p style="text-align: justify; text-indent: 2em;">A seguir, descrevemos o que é cada elemento do diagrama de colaboração acima. </p>

#### Objetos

1. **:Chef Indica**
    - É o sistema principal ou a aplicação que gerencia as interações entre usuário, avaliações, restaurantes, e categorias.
    - Media todas as chamadas relacionadas a buscas, login, avaliação de restaurantes e categorias.

2. **:Restaurante**
    - Representa um restaurante cadastrado no sistema.
    - Armazena informações como nome, avaliações associadas, e a média das notas recebidas.
    - Permite ao sistema acessar suas avaliações e atualizar sua média conforme novas avaliações são feitas.

3. **:Categoria**
    - Representa categorias de restaurantes por tipo de culinária.
    - Participa principalmente no filtro e busca por categorias.

4. **:Usuário**
    - Representa o usuário do sistema que interage com ele para realizar ações como:
        - Buscar restaurantes.
        - Fazer login e logout.
        - Avaliar restaurantes.
        - Buscar categorias de restaurantes.

5. **r:Avaliação**
    - Representa uma avaliação feita por um usuário em um restaurante.
    - Cada avaliação está vinculada a um restaurante e armazena informações como notas e feedback textual.
    - Permite operações como visualizar ou excluir avaliações.

#### Mensagens(interações)

##### Descrição das mensagens

1. **Mensagens do Usuário para o Sistema (Chef Indica)**
    - <b>1.* buscarRestaurante()</b>: Usuário busca por restaurantes disponíveis no sistema.
    - <b>2 setUsuario()</b>: Caso o usuário não tenha uma conta, ele é registrado no sistema.
    - <b>3 realizarLogin()</b>: Usuário faz login para poder escrever avaliações.
    - <b>3.4 realizarLogout()</b>: Usuário encerra a sessão no sistema.
    - <b>4.* buscarCategoria()</b>: Usuário busca categorias de restaurantes.

2. **Mensagens do Sistema para :Restaurante**
    - <b>1.1 search()</b>: Realiza a busca por restaurantes.
    - <b>1.2* obterAvaliacoes()</b>: Obtém as avaliações associadas a um restaurante.
    - <b>1.3 obterMedia()</b>: Calcula a média das avaliações.
    - <b>1.4 atualizarMedia()</b>: Atualiza a média das avaliações após uma nova avaliação.

3. **Mensagens para :Categoria**
    - <b>4.2 filtrarCategoria()</b>: Filtra os restaurantes com base na categoria selecionada.

4. **Mensagens Relacionadas a Avaliações (r:Avaliação)**
    - <b>1.7 viewAvaliação()</b>: Exibe as avaliações feitas para um restaurante.
    - <b>3.2* avaliarRestaurante()</b>: Permite que o usuário avalie um restaurante.
    - <b>3.3 apagarAvaliacoes()</b>: Exclui uma avaliação feita pelo usuário.

##### Fluxo de interações

1. **Busca de Restaurantes**
    - O usuário inicia a busca por restaurantes chamando o método buscarRestaurante() (mensagem 1.*).
    - O sistema (:Chef Indica) encaminha a busca para a instância :Restaurante, que realiza a operação search() (mensagem 1.1).
    - O resultado é apresentado ao usuário através do método viewRestaurante() (mensagem 1.5).

2. **Visualização e Cálculo de Avaliações**
    - Ao buscar por restaurantes, o sistema obtém as avaliações associadas ao restaurante por meio de obterAvaliacoes() (mensagem 1.2*).
    - A média das avaliações é calculada com o método obterMedia() (mensagem 1.3).
    - Caso novas avaliações sejam adicionadas, a média é atualizada pelo sistema através de atualizarMedia() (mensagem 1.4).

3. **Cadastro e Login do Usuário**
    - Se o usuário não possuir uma conta no sistema, ele será registrado com o método setUsuario() (mensagem 2).
    - Caso queira avaliar um restaurante, o usuário realiza login no sistema chamando realizarLogin() (mensagem 3).

4. **Avaliação de Restaurantes**
    - O usuário escolhe um restaurante para avaliar e executa o método avaliarRestaurante() (mensagem 3.2*).
    - Se o usuário decidir excluir uma avaliação, o sistema executa apagarAvaliacoes() (mensagem 3.3).

5. **Busca de Categorias**
    - O usuário pode buscar por categorias no sistema chamando o método buscarCategoria() (mensagem 4.*).
    - O sistema interage com a instância :Categoria para filtrar os resultados com o método filtrarCategoria() (mensagem 4.2).

6. **Logout**
    - Após realizar as ações desejadas, o usuário pode encerrar sua sessão chamando o método realizarLogout() (mensagem 3.4).

## Referências Bibliográficas

>DIAGRAMAS de colaboração UML, exemplos gratuitos e download de software. [S. l.], 25 out. 2024. Disponível em: https://www.edrawsoft.com/pt/uml-collaboration.html. Acesso em: 26 nov. 2024.
>
>GUIA: Diagramas de colaboração UML. [S. l.]. Disponível em: https://miro.com/pt/diagrama/o-que-e-diagrama-colaboracao-uml/. Acesso em: 26 nov. 2024
>
>UML Communication Diagrams Overview. [S. l.]. Disponível em: https://www.uml-diagrams.org/communication-diagrams.html. Acesso em: 26 nov. 2024.
>
>DIAGRAMA de Colaboração. [S. l.]. Disponível em: https://www.inf.ufpr.br/silvia/ES/projeto/aulas/aula14.pdf. Acesso em: 26 nov. 2024.
>
>06B - VideoAula - DSW-Modelagem - Comunicacao. Direção: Milene Serrano. [S. l.: s. n.], 2020. Disponível em: https://unbbr-my.sharepoint.com/personal/mileneserrano_unb_br/_layouts/15/stream.aspx?id=%2Fpersonal%2Fmileneserrano%5Funb%5Fbr%2FDocuments%2FArqDSW%20%2D%20V%C3%ADdeosOriginais%2F06b%20%2D%20VideoAula%20%2D%20DSW%2DModelagem%20%2D%20Comunicacao%2Emp4&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eb60ec98f%2D6a2e%2D4a1c%2Da6a3%2D7a9f14007014. Acesso em: 26 nov. 2024.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |26/11/2024| Adição da Introdução e Metodologia | [Guilherme Brito](https://github.com/GuilhermeB12)<br>[Júlia Yoshida](https://github.com/juliaryoshida)<br>[Maria Alice](https://github.com/Maliz30)<br> | [Mateus Fidelis](https://github.com/matsfidelis) |
| `1.1`  |27/11/2024| Detalhamento da metodologia | [Júlia Yoshida](https://github.com/juliaryoshida)| [Maria Alice](https://github.com/Maliz30) |
