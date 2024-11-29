# Diagrama de Casos de Uso

## Introdução
O diagrama de casos de uso é uma representação visual que modela as interações entre os atores externos e o sistema, destacando os principais serviços ou funcionalidades oferecidos. Ele descreve o comportamento do sistema do ponto de vista do usuário, auxiliando na definição de requisitos funcionais. No contexto de um site de recomendações de restaurantes, esse tipo de diagrama é valioso para mapear interações como buscar informações sobre restaurantes avaliados ou registrar novas avaliações.

Além de facilitar a modelagem dos cenários principais de uso, o diagrama de casos de uso também desempenha um papel importante na comunicação com stakeholders, apresentando de forma simplificada as funcionalidades e serviços planejados. Por isso, é amplamente utilizado desde as etapas iniciais da coleta de requisitos, como em entrevistas, reuniões e workshops. Ele também serve como documentação gráfica do escopo funcional, oferecendo aos gerentes de projetos uma visão organizada e acessível sobre as funcionalidades que o sistema deve implementar. [1]

## Metodologia
A construção dos casos de uso do site de recomendação de restaurantes ChefIndica foi feita baseada nos cenários criados na Entrega 01 da disciplina. Primeiro, foram definidos dois atores que interagem com o sistema: o usuário que cadastra uma avaliação/recomendação de um restaurante e o usuário que pesquisa um determinado restaurante, seja pelo nome, seja pela categoria, e visualiza suas recomendações e avaliações. Após a definição de todos os casos de uso, criou-se o diagrama na plataforma Lucid Chart de forma colaborativa com os elementos gráficos padrões de um Caso de Uso (Tabela 1) e seus respectivos relacionamentos seguindo o guia da plataforma Lucid Chart [2].

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 1:</b> Legenda do diagrama de caso de uso</p></font>

<table>
  <thead>
    <tr>
      <th>Elemento</th>
      <th>Nome</th>
      <th>Função</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><figure class="usecaseElement" style="width: 20%; display: flex;"><img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/uc-ator.drawio.png?raw=true" alt="Ator"></figure></td>
      <td>Ator</td>
      <td>Representam os diferentes tipos de usuários externos que interagem com o sistema</td>
    </tr>
    <tr>
      <td><figure class="usecaseElement" style="width: 40%; display: flex;"><img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/uc-caso-de-uso.drawio.png?raw=true" alt="Elipse (Caso de Uso)"></figure></td>
      <td>Elipse (Caso de Uso)</td>
      <td>É usada para representar os casos de uso no diagrama. Um caso de uso descreve uma funcionalidade ou uma ação específica que o sistema pode realizar em resposta às interações dos atores. A elipse contém o nome do caso de uso</td>
    </tr>
    <tr>
      <td><figure class="usecaseElement" style="width: 40%; display: flex;"><img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/uc-limites.drawio.png?raw=true" alt="Retângulo (Sistema)"></figure></td>
      <td>Retângulo (Sistema)</td>
      <td>Usado para representar o sistema ou o bloco em análise. Ele envolve os casos de uso e atores relacionados</td>
    </tr>
    <tr>
      <td><figure class="usecaseElement" style="width: 40%; display: flex;"><img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/uc-relacionamentos.drawio.png?raw=true" alt="Flecha (Relações)"></figure></td>
      <td>Flecha (Relações)</td>
      <td>As flechas são usadas para representar as relações ou interações entre atores e casos de uso</td>
    </tr>
  </tbody>
</table>

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Victor</a>, 2024</p></font>
</div>

## Diagrama de Casos de Uso

A figura 1 demonstra o diagrama de casos de uso resultante.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 1:</b> Diagrama de caso de uso do site ChefIndica</p></font>

<img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/diagrama-de-cdu.png" class="usecaseElement" width="80%">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Caiomesvie">Caio Mesquita</a>, <a href="https://github.com/cqcoding">Cecília Quaresma</a>, <a href="https://github.com/VieiraLaris">Larissa Vieira</a>, <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, <a href="https://github.com/lucas13032003">Lucas Victor</a>, <a href="https://github.com/Maliz30">Maria Alice</a> e <a href="https://github.com/zenildavieira">Zenilda Vieira</a>, 2024</p></font>

</div>

## Especificação dos Casos de Uso

### UC01.0 Fazer login

A tabela 2 demonstra a especificação do caso de uso UC01.0 Fazer login.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 2:</b> Especificação do caso de uso UC01.0</p></font>
</div>

| UC01.0 |  Fazer login |
| --- | --- |
| **Ator(es)** | Usuário que vai cadastrar uma avaliação e/ou recomendação.|
| **Frequência de uso** | Média |
| **Pré-condições** | PRE01. Dispor de uma conexão à internet;<br> PRE02. Usuário abrir o site deslogado.|
| **Fluxo básico** | <b>FB01. </b> <ol> <li> O usuário fornece seus dados de login. Aciona o caso de uso UC01.2.<li> O usuário é logado. <li> Fim do caso de uso. </ol> |
| **Fluxos alternativos** | --- |
| **Fluxos de exceção** | <b>FE01: Dados do login errados </b> <ol> <li> O usuário fornece algum dado do login errado <li> O sistema informa qual campo está com o dado inválido. Aciona o caso de uso UC01.1. </ul> </ol> |
| **Pós-condições** |POS01. O usuário é logado em sua conta do site. |
| **Data da criação** | 19/11/2024 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div >

### UC01.1. Exibir erro de login

A tabela 3 demonstra a especificação do caso de uso UC01.1 Exibir erro de login.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 3:</b> Especificação do caso de uso UC01.1</p></font>
</div>

| UC01.1 | Exibir erro de login |
| -: | :- |
| **Ator(es)** | Sistema |
| **Frequência de uso** | Baixa |
| **Pré-condições** | PRE01. O usuário forneceu algum dado errado no login.|
| **Fluxo básico** |<b>FB01. </b> <ol> <li> O usuário fornece seus dados de login. Aciona o caso de uso UC01.2. <li> O sistema informa em qual campo o usuário forneceu um dado inválido </ol> |
| **Fluxos alternativos** | --- |
| **Fluxos de exceção** | --- |
| **Pós-condições** |POS01. O usuário deve colocar novamente suas credenciais de login. |
| **Data da criação** | 19/11/2024 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div >

### UC01.2. Verificar dados de login

A tabela 4 demonstra a especificação do caso de uso UC01.2 Verificar dados de login.

<div align="center">  
<font size="3"><p style="text-align: center"><b>Tabela 4:</b> Especificação do caso de uso UC01.2</p></font>
</div>

| UC01.2 |  Verificar dados de login |
| -: | :- |
| **Ator(es)** | Sistema |
| **Frequência de uso** | Média |
| **Pré-condições** | PRE01. O usuário fornceceu os dados de login.|
| **Fluxo básico** |<b>FB01. </b> <ol> <li> O sistema recebe os dados que o usuário forneceu. <li> O sistema verifica os dados de login. <li> O sistema libera o login do usuário. <li> Fim do caso de uso. |
| **Fluxos alternativos** | --- |
| **Fluxos de exceção** | <b>FE01: Dados do login errados </b> <ol> <li> O usuário fornece algum dado do login errado. <li> O sistema verifica os dados de login. aciona o caso de uso UC01.1. <li> O sistema não permite o login do usuário. Aciona o caso de uso UC01. <li> Fim do caso de uso. </ul> </ol> |
| **Pós-condições** |POS01. O usuário é logado em sua conta do aplicativo. |
| **Data da criação** |19/11/2024 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div >

### UC02. Fazer Cadastro Usuário

A tabela 5 demonstra a especificação do caso de uso UC02 Fazer Cadastro Usuário.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 5:</b> Especificação do caso de uso UC02</p></font>
</div>

| UC02 | Fazer Cadastro Usuário |
| -: | :- |
| **Ator(es)** | Usuário que deseja criar uma conta no sistema para avaliar ou comentar restaurantes. |
| **Frequência de uso** | Alta |
| **Pré-condições** | PRE01. O usuário deve ter acesso à internet;<br> PRE02. O sistema deve estar disponível;<br> PRE03. O usuário deve acessar a página de um restaurante no site. |
| **Fluxo básico** | <b>FB01.</b> <ol> <li> O usuário acessa a página de um restaurante avaliado. <li> O usuário decide avaliar ou comentar. <li> O sistema redireciona para a página de login/cadastro. <li> O usuário escolhe criar uma nova conta. <li> O usuário preenche os campos obrigatórios (nome, e-mail, senha, etc.). <li> O sistema valida as informações fornecidas. <li> O sistema cria a conta do usuário. <li> O sistema redireciona o usuário à página do restaurante. <li> O usuário realiza a avaliação ou comentário. <li> Fim do caso de uso. </ol> |
| **Fluxos alternativos** | <b>FA01: E-mail já cadastrado</b> <ol> <li> O sistema detecta que o e-mail informado já está cadastrado. <li> O sistema exibe uma mensagem informando o erro e solicita um novo e-mail. <li> Retorna ao passo FB05. </ol> |
| **Fluxos de exceção** | <b>FE01: Falha de conexão</b> <ol> <li> O sistema não consegue conectar ao servidor. <li> O sistema exibe uma mensagem informando a indisponibilidade temporária. <li> Fim do caso de uso. </ol> |
| **Pós-condições** | POS01. O usuário possui uma conta cadastrada no sistema e consegue realizar avaliações ou comentários. |
| **Data da criação** | 21/11/2024 |

<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/lucas13032003">Lucas Victor</a>, 2024</p></font>
</div >


### UC03. Avaliar Restaurante

A tabela 6 demonstra a especificação do caso de uso UC03 Avaliar Restaurante.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 6:</b> Especificação do caso de uso UC03</p></font>
</div>

| UC03 |  Avaliar Restaurante |
| -: | :- |
| **Ator(es)** | Usuário |
| **Frequência de uso** | Baixa |
| **Pré-condições** | PRE01. Dispor de uma conexão à internet.<br>PRE02. Usuário estar logado no aplicativo.|
| **Fluxo básico** | <br>**FB01.**</br> <ol> <li>O usuário realiza uma pesquisa de restaurantes no aplicativo.<li>O usuário seleciona um restaurante da lista de resultados.<li>O sistema exibe as informações detalhadas do restaurante selecionado.<li>O usuário seleciona a opção “Comentar”.<li>O sistema exibe os campos para a nota e o comentário.<li>O usuário fornece a nota e, opcionalmente, um comentário.<li>O usuário clica em "Avaliar".<li>O sistema registra a avaliação.<li>Fim do caso de uso. </ol>|
| **Fluxos alternativos** | <br>**FA01: Avaliar sem comentário**</br>  <ol> <li>O usuário escolhe apenas a nota e não fornece comentário.<li>O sistema registra a avaliação com a nota e sem comentário.<li>Fim do caso de uso. </br>|
| **Fluxos de exceção** | <br>**FE01: Falha ao registrar avaliação**</br> <ol> <li>O sistema não consegue registrar a avaliação devido a erro de comunicação ou outro erro técnico.<li>O sistema informa que houve um erro e solicita ao usuário tentar novamente. </ol><br>**FE02: Usuário não logado**</br> <ol> <li>O usuário tenta avaliar sem estar logado.<li>O sistema informa que é necessário estar logado para avaliar. O usuário é direcionado para a tela de login. </ol>|
| **Pós-condições** | POS01. A avaliação do restaurante foi registrada com sucesso. |
| **Data da criação** |20/11/2024|


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/VieiraLaris">Larissa Vieira</a>, 2024</p></font>
</div >

### UC04.  Fazer Comentário

A tabela 7 demonstra a especificação do caso de uso UC04  Fazer Comentário.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 7:</b> Especificação do caso de uso UC04</p></font>
</div>

| UC04 |  Fazer Comentário |
| -: | :- |
| **Ator(es)** | Usuário que vai deixar um comentário sobre um restaurante |
| **Frequência de uso** | Baixa |
| **Pré-condições** | PRE01. Dispor de uma conexão à internet;<br> PRE02. Usuário deve estar logado no site;<br> PRE03. O sistema deve estar disponível;<br> PRE04. O usuário deve acessar a página de um restaurante no site.<br> PRE05. Usuário avaliar um restaurante; |
| **Fluxo básico** | <br>**FB01.**</br> <ol> <li>O usuário pesquisa um restaurante listado no aplicativo.<li>O usuário seleciona um restaurante da lista de resultados.<li>O sistema exibe as informações detalhadas do restaurante selecionado.<li>O usuário seleciona a opção “Comentar”.<li>O sistema exibe os campos para a nota e o comentário.<li>O usuário fornece a nota e registra seu comentário.<li>O usuário clica em "Avaliar".<li>O sistema registra a avaliação.<li>Fim do caso de uso. </ol>|
| **Fluxos alternativos** | <br>**FA01. Restaurante não encontrado**</br><ol><li>O usuário pesquisa por um restaurante que não está listado.<li> O sistema informa que o restaurante não foi encontrado e oferece a opção de sugerir a adição do restaurante ao sistema.<li> O usuário deicde se deseja ou não sugerir o restaurante.<li> O caso de uso retorna ao fluxo básico FB01 caso o usuário pesquisa novamente.</ol> |
| **Fluxos de exceção** | <br>**FE01: Campo de avaliação vazio**</br> <ol> <li>O sistema não consegue prosseguir com o comentário caso não haja registro da avaliação do restraurante.<li> O usuário volta no campo de avaliação e clica na quantidade de estrelas correspondente à avaliação do restaurante</ol><br>**FE02: Usuário não logado**</br> <ol> <li>O usuário tenta avaliar sem estar logado.<li>O sistema informa que é necessário estar logado para avaliar. O usuário é direcionado para a tela de login. </ol>|
| **Pós-condições** | POS01. O comentário é realizado com sucesso e demais usuários podem visualizar. |
| **Data da criação** | 21/11/2024 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/cqcoding">Cecília Quaresma</a>, 2024</p></font>
</div >

### UC05. Pesquisar por Restaurante

A tabela 8 demonstra a especificação do caso de uso UC05 Pesquisar por Restaurante.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 8:</b> Especificação do caso de uso UC05</p></font>
</div>

| UC05 |  Pesquisar por Restaurante |
| -: | :- |
| **Ator(es)** | Usuário em busca de um restaurante  |
| **Frequência de uso** | Alta |
| **Pré-condições** |PRE01. Dispor de uma conexão à internet;<br> PRE02. O sistema deve estar disponível; |
| **Fluxo básico** | <br>**FB01.**</br> <ol> <li>O usuário entra no site.<li>O usuário seleciona a categoria desejada de restaurante no menu lateral<li>O usuário navega pela lista de restaurantes listados na categoria selecionada.<li>O usuário seleciona o restaurante desejado. <li>O usuário analisa a avaliação e os comentários a respeito do restaurante. </ol> |
| **Fluxos alternativos** | <br>**FA01. Busca por restaurante específico**</br><ol> <li>O usuário acessa o site. <li>O usuário acessa o menu de busca na parte superior da página. <li>O usuário Procura pelo restaurante específico.<li>O usuário analisa a avaliação e os comentários a respeito do restaurante.</ol><br> **FA02. Restaurante Recomendado** </br><ol><li>O usuário acessa o site. <li> O usuário vizualiza os restaurantes recomendados na página home com maior avaliação. <li>O usuário seleciona o restaurante desejado e vizualiza sua avaliação.  </ol> |
| **Fluxos de exceção** | <br>**FE01: Restaurante não encontrado**</br> <ol> <li> O usuário busca pela avaliação de um restaurante em específico. <li> O usuário não encontra o restaurante cadastrado. <li> O usuário tem a opção de cadastrar o restaurante na plataforma. </ol> |
| **Pós-condições** | POS01. O usuário vizualiza a avaliação do restaurante selecionado.  |
| **Data da criação** |26/11/2024 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Caiomesvie">Caio Mesquita</a>, 2024</p></font>
</div > 

### UC06. Filtrar Restaurantes por Categoria

A tabela 9 demonstra a especificação do caso de uso UC06 Filtrar por Categoria.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 9:</b> Especificação do caso de uso UC06</p></font>
</div>

| UC06 |  Filtrar Restaurantes por Categoria |
| -: | :- |
| **Ator(es)** |  Usuário que deseja encontrar restaurantes de categorias específicas (Categorias listadas abaixo desta tabela*).       |
| **Frequência de uso** |  Alta |
| **Pré-condições** | PRE01. O usuário deve ter acesso à internet;<br>PRE02. O sistema deve estar disponível;<br>PRE03. O usuário deve acessar a página de busca de restaurantes.                          |
| **Fluxo básico** | **FB** <br> 1. O usuário acessa a página de busca de restaurantes.<br>2. O usuário seleciona uma ou mais categorias para o filtro.<br>3. O sistema aplica os filtros selecionados.<br>4. O sistema exibe os restaurantes que correspondem as categorias escolhidas.<br>5. O usuário visualiza os resultados e pode acessar um restaurante.<br>6. Fim do caso de uso.|
| **Fluxos alternativos** | **FA01: Nenhum restaurante encontrado**<br>1. O sistema não encontra restaurantes que correspondam as categorias escolhidas.<br>2. O sistema exibe uma mensagem informando que não há resultados.<br>3. O usuário pode redefinir os filtros.<br>4. Retorna ao passo FB02.                                                                                   |
| **Fluxos de exceção** | **FE01: Falha de conexão**<br>1. O sistema não consegue carregar os resultados da busca.<br>2. O sistema exibe uma mensagem informando a indisponibilidade temporária.<br>3. Fim do caso de uso. |
| **Pós-condições** | POS01. O sistema exibe uma listagem dos restaurantes de acordo com a categoria selecionada ou informa a ausência de resultados com base na categoria escolhida.              |
| **Data da criação** | 27/11/24 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Maliz30">Maria Alice</a>, 2024</p></font>
</div >

**Categorias:** Brasileira, Japonesa, Chinesa, Italiana, Árabe, Doces e sobremesas, Mexicana, Fast-food, Padaria/Café, Hambúrguer, Lámen, Pizza, Bolos, Sorvete, Café da manhã, Vegano, Sem glúten, Vegetariano, Bebidas, Self-service, Churrasco ou Frutos do mar.

### UC06.1. Exibir listagem de restaurantes da categoria
A tabela 10 demonstra a especificação do caso de uso UC06.1 Exibir listagem de restaurantes da categoria.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 10:</b> Especificação do caso de uso UC06.1</p></font>
</div>

| UC06.1 |  Exibir listagem de restaurantes da categoria |
| -: | :- |
| **Ator(es)** | Sistema |
| **Frequência de uso** | Alta |
| **Pré-condições** | PRE01. Haverem restaurantes cadastrados para a categoria escolhida. |
| **Fluxo básico** | **FB** <br> 1. O usuário filtra restaurantes usando uma ou mais categorias. <br>2. O sistema exibe uma listagem de restaurantes que correspondem as categorias selecionada. |
| **Fluxos alternativos** | --- |
| **Fluxos de exceção** | **FE01: Falha de conexão**<br>1. O sistema não consegue carregar os resultados da busca.<br>2. O sistema exibe uma mensagem informando a indisponibilidade temporária.<br>3. Fim do caso de uso. |
| **Pós-condições** | POS01. O usuário visualiza uma listagem contendo todos os restaurantes cadastrados na categoria escolhida. |
| **Data da criação** | 27/11/24 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Maliz30">Maria Alice</a>, 2024</p></font>
</div >

### UC06.2. Exibir mensagem informado a ausência de restaurantes

A tabela 11 demonstra a especificação do caso de uso UC06.2 Exibir mensagem informado a ausência de restaurantes.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 11:</b> Especificação do caso de uso UC06.2</p></font>
</div>

| UC06.2 |  Exibir mensagem informado a ausência de restaurantes |
| -: | :- |
| **Ator(es)** | Sistema |
| **Frequência de uso** | Média |
| **Pré-condições** | PRE01. Não haverem restaurantes cadastrados para a categoria escolhida. |
| **Fluxo básico** | **FB** <br> 1. O usuário filtra restaurantes usando uma ou mais categorias. <br>2. O sistema informa que não há restaurantes com essas categorias na base de dados. |
| **Fluxos alternativos** | --- |
| **Fluxos de exceção** | --- |
| **Pós-condições** | POS01. O sistema exibe uma mensagem informando que não há resultados cadastrados para aquela categoria; <br> POS02. O usuário cadastra um restaurante na categoria escolhida. |
| **Data da criação** | 27/11/24 |


<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Maliz30">Maria Alice</a>, 2024</p></font>
</div >

### UC07. Cadastrar Restaurante

A tabela 12 demonstra a especificação do caso de uso UC07 Cadastrar Restaurante.

<div align="center">
<font size="3"><p style="text-align: center"><b>Tabela 12:</b> Especificação do caso de uso UC07</p></font>
</div>

| UC07 |  Cadastrar Restaurante |
| -: | :- |
| **Ator(es)** | Usuário |
| **Frequência de uso** | Média |
| **Pré-condições** | PRE01. O usuário deve estar logado no aplicativo. <br> PRE02. Dispor de uma conexão à internet. |
| **Fluxo básico** | <br>**FB01.**</br> <ol> <li>O usuário acessa a opção "Cadastrar Restaurante" no menu do aplicativo.<li> O sistema exibe um formulário para preenchimento.<li>O usuário insere as informações necessárias, como foto, nome, local e categoria. <li>O usuário confirma o cadastro clicando em "Adicionar".<li>O sistema valida os dados fornecidos. <li>O sistema registra o restaurante na base de dados. <li>O sistema exibe uma mensagem de sucesso confirmando o cadastro. <li>Fim do caso de uso. </ol>|
| **Fluxos alternativos** | <br>**FA01: Restaurante já cadastrado**</br>  <ol> <li>O sistema verifica que o restaurante informado já existe na base de dados.<li>O sistema exibe uma mensagem informando que o restaurante já está cadastrado e sugere ao usuário verificar as informações ou buscar diretamente pelo nome.<li>O sistema não permite um novo cadastro para o mesmo restaurante.<li>Fim do caso de uso. </br>|
| **Fluxos de exceção** | <br>**FE01: Falha na validação dos dados**</br>  <ol> <li>O sistema identifica que um ou mais campos obrigatórios estão ausentes ou preenchidos incorretamente.<li>O sistema informa ao usuário quais campos precisam ser corrigidos e solicita a revisão dos dados.<li>O usuário corrige os dados e tenta novamente.<li>Fim do caso de uso. </ol><br>**FE02: Falha ao registrar o restaurante**</br>  <ol> <li>O sistema não consegue registrar o restaurante devido a erro técnico ou falta de conexão com a base de dados.<li>O sistema exibe uma mensagem de erro ao usuário e solicita que ele tente novamente mais tarde.<li>Fim do caso de uso. </ol> |
| **Pós-condições** | POS01. O restaurante foi cadastrado com sucesso e está disponível para consulta no aplicativo. |
| **Data da criação** | 21/11/2024 |

<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div >


## Referências Bibliográficas

> [1] REINEHR, Sheila. Engenharia de requisitos. Porto Alegre: Grupo A, 2020. E-book. ISBN 9786556900674. Disponível em: <https://integrada.minhabiblioteca.com.br/#/books/9786556900674/>. Acesso em: 19 de novembro de 2024.
> 
> [2] Lucid Software Português. Tutorial de Caso de Uso UML [Recurso eletrônico: vídeo], 2019.  Disponível em: <https://www.youtube.com/watch?v=ab6eDdwS3rA>.  Acesso em: 19 de novembro de 2024.


## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |18/11/2024| Adição da introdução | [Luana Medeiros](https://github.com/LuaMedeiros) | [Zenilda Vieira](https://github.com/zenildavieira) |
| `1.1`  |19/11/2024| Complementação da introdução, inclusão da metodologia, <br> criação do padrão das tabelas de especificações e inclusão do caso de uso UC01 | [Zenilda Vieira](https://github.com/zenildavieira) | [Luana Medeiros](https://github.com/LuaMedeiros) |
| `1.2`  |20/11/2024| Adição do caso de uso UC03 | [Larissa Vieira](https://github.com/VieiraLaris) | [Luana Medeiros](https://github.com/LuaMedeiros) |
| `1.3`  |21/11/2024| Adição do caso de uso UC07 | [Luana Medeiros](https://github.com/LuaMedeiros) | [Lucas Víctor](https://github.com/Lucas3032003) |
| `1.4`  |21/11/2024| Adição do caso de uso UC02  | [Lucas Víctor](https://github.com/Lucas3032003) |  [Luana Medeiros](https://github.com/LuaMedeiros)|
| `1.5`  |21/11/2024| Adição do caso de uso UC04  | [Cecília Quaresma](https://github.com/cqcoding) | [Caio Mesquita](https://github.com/Caiomesvie) |
| `1.6`  |27/11/2024| Adição do caso de uso UC05  |  [Caio Mesquita](https://github.com/Caiomesvie) | [Cecília Quaresma](https://github.com/cqcoding)|
| `1.7`  |27/11/2024| Adição do novo diagrama | [Cecília Quaresma](https://github.com/cqcoding)| [Maria Alice](https://github.com/Maliz30) |
| `1.8`  |27/11/2024| Adição de especificação de casos de uso UC06 | [Maria Alice](https://github.com/Maliz30) | [Cecília Quaresma](https://github.com/cqcoding) |
| `1.9`  |28/11/2024| Atualização de legenda  | [Lucas Víctor](https://github.com/Lucas3032003) |  [Luana Medeiros](https://github.com/LuaMedeiros)|
| `2.0`  | 28/11/2024 | Correção de alguns links de figuras | [Zenilda Vieira](https://github.com/ZenildaVieira) |  |