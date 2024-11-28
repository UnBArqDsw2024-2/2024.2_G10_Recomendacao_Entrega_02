# NFR Framework

## Introdução 

### Definição

O **NFR (Non-Functional Requirements) Framework**, ou *Framework de Requisitos Não Funcionais*, é uma abordagem essencial no desenvolvimento de software e engenharia de sistemas. Para o *Chefindica* — site de indicação e avaliação de restaurantes — este framework ajuda a definir e gerenciar requisitos que não estão diretamente ligados às funcionalidades específicas do sistema (como a busca ou cadastro de restaurantes), mas sim às características que impactam a qualidade geral do software. Entre essas características estão o desempenho, a segurança, a usabilidade e a experiência do usuário. Esses requisitos não funcionais (NFRs) desempenham um papel essencial ao determinar como o sistema deve se comportar para oferecer uma experiência eficiente, confiável e agradável para os usuários, garantindo, por exemplo, tempos de resposta rápidos ao buscar restaurantes, proteção de dados pessoais ao avaliar estabelecimentos e interfaces intuitivas para navegação.

O NFR Framework utiliza o conceito de "softgoal", que se refere a um objetivo que não possui critérios de satisfação estritamente definidos. Os softgoals podem estar conectados, refletindo como um requisito influencia outro, como, por exemplo, como a "segurança de dados" influencia a "confidencialidade das avaliações". Desa forma, esse framework permite:

1. Organização e priorização: Os RNFs, como desempenho, segurança, usabilidade e confiabilidade, são organizados em hierarquias para facilitar a visualização.
2. Análise de impacto: Mostra como decisões de design atendem aos RNFs e quais compromissos (trade-offs) são necessários.
3. Rastreabilidade: Facilita o rastreamento dos RNFs ao longo do ciclo de desenvolvimento do software.
4. Documentação visual: Usa representações gráficas (softgoal interdependency graphs) para mostrar as interdependências e os níveis de satisfação dos RNFs. 

O **NFR Framework** organiza essas conexões em gráficos chamados *Softgoal Interdependency Graphs (SIGs)*. Esses gráficos registram as considerações dos desenvolvedores sobre os softgoals e suas interdependências. No caso do *Chefindica*, os SIGs podem detalhar decisões sobre requisitos como: 

- **Tempo de Resposta**: O sistema deve retornar sugestões de restaurantes em menos de 2 segundos.  
- **Privacidade do Usuário**: Garantir que as avaliações sejam armazenadas de forma anônima.  
- **Acessibilidade**: Tornar o sistema acessível para usuários com deficiência visual.  

O SIG também ajuda a justificar as escolhas feitas durante o desenvolvimento, facilitando a avaliação de alto nível para garantir que os requisitos não funcionais sejam atendidos.

### Tipos de Softgoals 

Os softgoals no NFR Framework se dividem em três categorias principais, que são representadas no gráfico de interdependência. Esses softgoals podem ser caracterizados da seguinte forma:  

1. **Softgoals NFR**:  
   Representam os requisitos não funcionais principais do sistema. São características abstratas, as quais vão ser analisadas para saber se serão escolhidas ou não para serem implementadas.  
   - Exemplo no *Chefindica*: "Garantir baixa latência no carregamento da página inicial".  

2. **Softgoals de Operacionalização**:  
   Correspondem às soluções de implementação para alcançar os softgoals NFR ou outros softgoals de operacionalização, ou seja, são as funcionalidades.  
   - Exemplo no *Chefindica*: "Implementar cache local para reduzir o tempo de busca de restaurantes".  

3. **Softgoals de Afirmação**:  
   Levam em conta as características do domínio, como prioridades do sistema ou comportamento dos usuários. São anotações escritas em linguagem natural, explicitando algum ponto específico da modelagem. 
   - Exemplo no *Chefindica*: "Priorizar a segurança dos dados dos usuários em detrimento de algumas otimizações de desempenho".  

A **Figura 1** abaixo ilustra a representação dos tipos de softgoals, que pode ser utilizada como legenda para os gráficos SIGs do *Chefindica*.  

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 1:</b> Representação dos tipos de softgoal adaptados para o *Chefindica*.</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/nfr-softgoals.png" style="width: 30%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> (CHUNG et al., 2000).</a></p></font>
</div>

### Avaliação e Propagação de Impactos  

No NFR Framework, a avaliação e a propagação de impactos analisa como as decisões tomadas para atender a um requisito específico influenciam outros requisitos dentro do sistema. Essa abordagem é especialmente útil para identificar e gerenciar compromissos (trade-offs) entre os RNFs durante o processo de design.  Isso ocorre por meio da atribuição de rótulos aos softgoals nos SIGs, que representam os RNFs e suas interdependências. No *Chefindica*, o processo de avaliação pode verificar, por exemplo:

- O tempo médio de resposta atende aos 2 segundos especificados?  
- A implementação de criptografia garante a privacidade dos dados?  
- A interface de acessibilidade permite o uso por pessoas com deficiência?  

Os rótulos utilizados na avaliação e propagação de impactos descrevem o nível de satisfação dos requisitos e influências que podem ocorrer. São eles:
- **Satisfeito**: O softgoal pode ser cumprido (escolhido para ser implementado).  
- **Fracamente Satisfeito**: Há indicadores positivos para o cumprimento do softgoal.  
- **Negado**: O softgoal não pode ser cumprido (não escolhido para ser implementado).  
- **Fracamente Negado**: Há indicadores contras para o cumprimento total do softgoal.  
- **Conflitante**: Existem conflitos de interesse para o cumprimento do softgoal: alguns indicadores positivos e outros negativos.
- **Indeterminado**: O cumprimento do softgoal não pode ser confirmado nem negado.  

A **Figura 2** apresenta os rótulos de propagação de impactos que podem ser usados no SIG do *Chefindica*.  

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 2:</b> Rótulos de propagação de impactos adaptados ao *Chefindica*.</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/nfr-impactos.png" style="width: 65%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> (CHUNG et al., 2000).</a></p></font>
</div>

Com base nesses rótulos, é possível ajustar as prioridades e refinar a implementação para garantir que o *Chefindica* atenda às expectativas dos usuários e aos objetivos de qualidade definidos pelo NFR Framework.

## Metodologia

Neste documento, foram apresentadas 6 categorias de NFRs, que foram definidas a partir do documento de [Especificação Suplementar](https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md), que por sua vez se baseou no modelo FURPS+. Para cada categoria, foi feito um SIG (Softgoal Interdependency Graph), um diagrama da propagação de impactos e um cartão de especificação, que possui informações sobre os NFRs, como a descrição, a categoria, os conflitos, a origem, os critérios e outras informações. Os diagramas foram desenhados utilizando a ferramenta 

Os integrantes do grupo que participaram da elaboração desse documento foram os mesmos que elaboraram o documento de especificação suplementar: [Luana Medeiros](https://github.com/LuaMedeiros), [Lucas Victor](https://github.com/Lucas13032003) e [Zenilda Vieira](https://github.com/ZenildaVieira). A introdução e a metodologia foi elaborada pelo Lucas Victor e revisada/complementada por Zenilda. Em seguida, definiu-se que cada um ficaria responsável de criar o SIG, o diagrama de propagação de impactos e o cartão de especificação dos requisitos os quais foram responsáveis de elicitar. Dessa forma, os NFR Frameworks de usabilidade e confiabilidade foram elaborados pelo Lucas Víctor, os de desempenho e suporte pela Zenilda e os de restrições de design e ajuda/documentação pela Luana.

## NFR Framework

### NFR01 - Usabilidade 

**Usabilidade**, segundo Nielsen, é a medida de quão fácil e agradável é usar um sistema para alcançar os objetivos dos usuários. 


#### Softgoal Interdependency Graph

O _Softgoal Interdependency Graph_ do softgoal "Usabilidade" pode ser visto na figura 3.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 3:</b> Softgoal Interdependency Graph do softgoal "Usabilidade".</p></font>

<img src="/home/lv/Documentos/Chefindica/2024.2_G10_Recomendacao_Entrega_02/docs/imagens/Usanilidade_NFR.png" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>

#### Propagação de Impactos

A propagação de impactos do softgoal "Usabilidade" pode ser visto na figura 4.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 4:</b> Propagação de impactos do softgoal "Usabilidade"</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/imagens/w+.png?raw=true" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>


#### Cartão de Especificação  
Na tabela 1, temos o cartão de especificação do softgoal "Usabilidade".  

<div align="center">
<p><b>Tabela 1:</b> Cartão de Especificação do Softgoal Usabilidade</p>
<table>
  <tr>
    <th>Tópico</th>
    <th>Informação</th>
  </tr>
  <tr>
    <td>ID do NFR</td>
    <td>NFR01</td>
  </tr>
  <tr>
    <td>Classificação</td>
    <td>Usabilidade</td>
  </tr>
  <tr>
    <td>Descrição</td>
    <td>O requisito "Usabilidade" refere-se à capacidade do sistema de entregar uma boa usabilidade para os usuários do site "ChefIndica".</td>
  </tr>
  <tr>
    <td>Justificativa</td>
    <td>Uma boa usabilidade é fundamental para garantir que os usuários possam utilizar o site com eficiência e satisfação, promovendo acessibilidade e reduzindo erros.</td>
  </tr>
  <tr>
    <td>Origem do Requisito</td>
    <td><a href="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md">Especificação suplementar</a> e <a href="#">requisitos elicitados</a></td>
  </tr>
  <tr>
    <td>Dependências</td>
    <td>Não foram identificadas restrições ou dependências específicas, mas a atualização da documentação deve ser planejada e coordenada com as versões do site.</td>
  </tr>
  <tr>
    <td>Prioridade</td>
    <td>O requisito de "Usabilidade" é de alta prioridade, uma vez que influencia diretamente a satisfação do usuário e a eficácia do site.</td>
  </tr>
  <tr>
    <td>Conflitos</td>
    <td>Não foi identificado nenhum conflito.</td>
  </tr>
  <tr>
    <td>História</td>
    <td>21/11/2024</td>
  </tr>
</table>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>  


###  NFR02 - Confiabilidade (Reliability)

A "Confiabilidade" é uma característica importante que se refere à capacidade do sistema de funcionar de maneira consistente, estável e sem falhas. Isso assegura que os usuários possam confiar que o site, no caso do _Chefindica_, estará disponível e operando corretamente sempre que precisarem utilizá-lo. A confiabilidade desempenha um papel essencial para garantir uma experiência positiva do usuário, evitando erros, interrupções inesperadas e mantendo a credibilidade do site. Como a "Ajuda e Documentação" são recursos essenciais para orientar os usuários, a confiabilidade é o alicerce que sustenta a confiança dos usuários no sistema, permitindo que eles utilizem as informações da "Ajuda e Documentação" com segurança e eficácia.

#### Softgoal Interdependency Graph

O _Softgoal Interdependency Graph_ do softgoal "Confiabilidade (Reliability)" pode ser visto na figura 5.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 5:</b> Softgoal Interdependency Graph do softgoal "Confiabilidade (Reliability)".</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/imagens/NFR%20-%20Page%201.png?raw=true" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>


#### Propagação de Impactos

A propagação de impactos do softgoal "Confiabilidade (Reliability)" pode ser visto na figura 6.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 6:</b> Propagação de impactos do softgoal "Confiabilidade (Reliability)"</p></font>

<img src="#" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>

#### Cartão de Especificação
Na tabela 2, temos o cartão de especificação do Softgoal "Confiabilidade (Reliability)".

<div align="center">
<p><b>Tabela 2:</b> Cartão de Especificação do Softgoal “Confiabilidade (Reliability)”</p>
<table>
  <tr>
    <th>Tópico</th>
    <th>Informação</th>
  </tr>
  <tr>
    <td>ID do NFR</td>
    <td>NFR02</td>
  </tr>
  <tr>
    <td>Classificação</td>
    <td>Confiabilidade</td>
  </tr>
  <tr>
    <td>Descrição</td>
    <td>O Softgoal "Confiabilidade" refere-se à capacidade do aplicativo de funcionar consistentemente, estável e sem falhas, garantindo uma experiência positiva do usuário e a credibilidade do aplicativo.</td>
  </tr>
  <tr>
    <td>Justificativa</td>
    <td>A Confiabilidade é fundamental para manter a satisfação do usuário, evitar interrupções inesperadas e garantir o funcionamento correto do aplicativo. Ela é essencial para a credibilidade do aplicativo.</td>
  </tr>
  <tr>
    <td>Origem do Requisito</td>
    <td><a href="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md">Especificação suplementar</a> e <a href="#">requisitos elicitados</a></td>
  </tr>
  <tr>
    <td>Dependências</td>
    <td>Não foram identificadas dependências específicas, mas a manutenção e atualização do aplicativo devem ser coordenadas com as versões lançadas.</td>
  </tr>
  <tr>
    <td>Prioridade</td>
    <td>O Softgoal de "Confiabilidade" é de alta prioridade devido ao seu impacto direto na satisfação do usuário e na credibilidade do aplicativo.</td>
  </tr>
  <tr>
    <td>Conflitos</td>
    <td>Não foi identificado nenhum conflito com outros requisitos.</td>
  </tr>
  <tr>
    <td>História</td>
    <td>04/11/2024</td>
  </tr>
</table>

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>

###  NFR03 - Desempenho (Performance)

Desempenho refere-se à capacidade do sistema de responder rapidamente às interações dos usuários, garantindo tempos de resposta ágeis e um uso eficiente de recursos computacionais. No ChefIndica, o desempenho é essencial para oferecer uma experiência fluida, particularmente ao realizar buscas, acessar informações de restaurantes e realizar operações críticas como login.

#### Softgoal Interdependency Graph

O _Softgoal Interdependency Graph_ do softgoal "Desempenho" organiza os elementos relacionados à eficiência do sistema, como tempos de carregamento, capacidade de processamento e uso de recursos (ver Figura 7). Ele ajuda a identificar e equilibrar as interdependências entre requisitos que afetam a velocidade e a eficiência do sistema.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 7:</b> Softgoal Interdependency Graph do softgoal "Desempenho (Performance)".</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/nfr-desempenho.png" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div>


#### Propagação de Impactos

No SIG de desempenho, a propagação de impactos permite avaliar como a otimização de uma área do sistema pode influenciar outros atributos. Por exemplo:

* Reduzir o tempo de resposta do sistema ao realizar buscas pode exigir maior capacidade de processamento, aumentando o custo operacional.
* Otimizações de carregamento podem melhorar a experiência do usuário, mas podem comprometer a escalabilidade em situações de alta demanda.

Essa análise ajuda a identificar soluções que maximizem a eficiência enquanto equilibram custos e limitações técnicas.A propagação de impactos do softgoal "Desempenho (Performance)" pode ser visto na figura 8.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 8:</b> Propagação de impactos do softgoal "Desempenho (Performance)"</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/nfr-desempenho-impactos.png" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div>

#### Cartão de Especificação
Na tabela 3, temos o cartão de especificação do Softgoal "Desempenho (Performance)".

<div align="center">
<p><b>Tabela 3:</b> Cartão de Especificação do Softgoal “Desempenho (Performance)”</p>
<table>
  <tr>
    <th>Tópico</th>
    <th>Informação</th>
  </tr>
  <tr>
    <td>ID do NFR</td>
    <td>NFR03</td>
  </tr>
  <tr>
    <td>Classificação</td>
    <td>Desempenho</td>
  </tr>
  <tr>
    <td>Descrição</td>
    <td>Refere-se à capacidade do sistema de realizar operações rapidamente, garantindo tempos de resposta curtos.</td>
  </tr>
  <tr>
    <td>Justificativa</td>
    <td>Um desempenho elevado é importante para garantir uma experiência fluida e responsiva para os usuários.</td>
  </tr>
  <tr>
    <td>Origem do Requisito</td>
    <td><a href="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md">Especificação suplementar</a> e <a href="#">requisitos elicitados</a></td>
  </tr>
  <tr>
    <td>Dependências</td>
    <td>Depende da utilização de algoritmos otimizados e infraestruturas escaláveis.</td>
  </tr>
  <tr>
    <td>Prioridade</td>
    <td>Alta, pois o desempenho impacta diretamente a usabilidade e a percepção de qualidade do sistema.</td>
  </tr>
  <tr>
    <td>Conflitos</td>
    <td>Não foi identificado conflito algum.</td>
  </tr>
  <tr>
    <td>História</td>
    <td>23/11/2024</td>
  </tr>
</table>

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div>


###  NFR04 - Suporte (Supportability)

Suporte refere-se à capacidade do sistema de ser facilmente mantido, monitorado e atualizado ao longo do tempo, garantindo que ele se adapte às mudanças de requisitos e continue a atender às necessidades dos usuários e desenvolvedores. No ChefIndica, isso envolve práticas como arquitetura modular, controle de versão e mecanismos para rastrear e corrigir erros rapidamente.

#### Softgoal Interdependency Graph

O Softgoal Interdependency Graph do softgoal "Suporte" organiza os elementos relacionados à manutenção e evolução do sistema, destacando atributos como modularidade, monitoramento e adaptabilidade (ver Figura 9). Essa estrutura permite entender as dependências entre requisitos que garantem o suporte contínuo ao sistema.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 9:</b> Softgoal Interdependency Graph do softgoal "Suporte (Supportability)".</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/nfr-suporte.png" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div>


#### Propagação de Impactos

No SIG de suporte, a propagação de impactos avalia como mudanças ou melhorias específicas afetam outros aspectos do sistema. Por exemplo:

* A implementação de uma arquitetura modular facilita futuras atualizações, mas pode aumentar a complexidade inicial do desenvolvimento.
* Garantir a integração de logs detalhados e rastreáveis melhora a capacidade de depuração, mas pode impactar o desempenho em situações de alta carga.

Essa análise ajuda a tomar decisões equilibradas, priorizando ações que minimizem impactos negativos e maximizem os benefícios para a manutenção do sistema. 

A propagação de impactos do softgoal "Suporte (Supportability)" pode ser visto na figura 10.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 10:</b> Propagação de impactos do softgoal "Suporte (Supportability)"</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/nfr-suporte-impactos.png" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div>

#### Cartão de Especificação
Na tabela 4, temos o cartão de especificação do Softgoal "Suporte (Supportability)".

<div align="center">
<p><b>Tabela 4:</b> Cartão de Especificação do Softgoal “Suporte (Supportability)”</p>
<table>
  <tr>
    <th>Tópico</th>
    <th>Informação</th>
  </tr>
  <tr>
    <td>ID do NFR</td>
    <td>NFR04</td>
  </tr>
  <tr>
    <td>Classificação</td>
    <td>Suporte</td>
  </tr>
  <tr>
    <td>Descrição</td>
    <td>Refere-se à capacidade do sistema de ser facilmente mantido e monitorado, com suporte a mudanças futuras.</td>
  </tr>
  <tr>
    <td>Justificativa</td>
    <td>Facilitar a evolução do sistema, corrigir problemas rapidamente e garantir continuidade operacional.</td>
  </tr>
  <tr>
    <td>Origem do Requisito</td>
    <td><a href="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md">Especificação suplementar</a> e <a href="#">requisitos elicitados</a></td>
  </tr>
  <tr>
    <td>Dependências</td>
    <td>Depende da adoção de práticas como arquitetura modular e controle de versão.</td>
  </tr>
  <tr>
    <td>Prioridade</td>
    <td>Alta, pois garante a capacidade de adaptação e manutenção do sistema ao longo do tempo.</td>
  </tr>
  <tr>
    <td>Conflitos</td>
    <td>Não foi identificado conflito algum.</td>
  </tr>
  <tr>
    <td>História</td>
    <td>23/11/2024</td>
  </tr>
</table>

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/ZenildaVieira">Zenilda Vieira</a>, 2024</p></font>
</div>

###  NFR05 - Restrições de Design

#### Softgoal Interdependency Graph

O _Softgoal Interdependency Graph_ do softgoal "Restrições de Design" pode ser visto na figura 11.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 11:</b> Softgoal Interdependency Graph do softgoal "Restrições de Design".</p></font>

<img src="#" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div>


#### Propagação de Impactos

A propagação de impactos do softgoal "Restrições de Design" pode ser visto na figura 12.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 12:</b> Propagação de impactos do softgoal "Restrições de Design"</p></font>

<img src="#" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div>


#### Cartão de Especificação
Na tabela 5, temos o cartão de especificação do Softgoal "Restrições de Design".

<div align="center">
<p><b>Tabela 5:</b> Cartão de Especificação do Softgoal “Restrições de Design”</p>
<table>
  <tr>
    <th>Tópico</th>
    <th>Informação</th>
  </tr>
  <tr>
    <td>ID do NFR</td>
    <td>NFR05</td>
  </tr>
  <tr>
    <td>Classificação</td>
    <td>Suporte</td>
  </tr>
  <tr>
    <td>Descrição</td>
    <td></td>
  </tr>
  <tr>
    <td>Justificativa</td>
    <td></td>
  </tr>
  <tr>
    <td>Origem do Requisito</td>
    <td><a href="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md">Especificação suplementar</a> e <a href="#">requisitos elicitados</a></td>
  </tr>
  <tr>
    <td>Dependências</td>
    <td></td>
  </tr>
  <tr>
    <td>Prioridade</td>
    <td></td>
  </tr>
  <tr>
    <td>Conflitos</td>
    <td></td>
  </tr>
  <tr>
    <td>História</td>
    <td>23/11/2024</td>
  </tr>
</table>

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div>

###  NFR06 - Ajuda e Documentação

#### Softgoal Interdependency Graph

O _Softgoal Interdependency Graph_ do softgoal "Ajuda e Documentação" pode ser visto na figura 11.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 11:</b> Softgoal Interdependency Graph do softgoal "Ajuda e Documentação".</p></font>

<img src="#" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div>


#### Propagação de Impactos

A propagação de impactos do softgoal "Ajuda e Documentação" pode ser visto na figura 112.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 12:</b> Propagação de impactos do softgoal "Ajuda e Documentação"</p></font>

<img src="#" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div>


#### Cartão de Especificação
Na tabela 6, temos o cartão de especificação do Softgoal "Ajuda e Documentação".

<div align="center">
<p><b>Tabela 6:</b> Cartão de Especificação do Softgoal “Ajuda e Documentação”</p>
<table>
  <tr>
    <th>Tópico</th>
    <th>Informação</th>
  </tr>
  <tr>
    <td>ID do NFR</td>
    <td>NFR05</td>
  </tr>
  <tr>
    <td>Classificação</td>
    <td>Suporte</td>
  </tr>
  <tr>
    <td>Descrição</td>
    <td></td>
  </tr>
  <tr>
    <td>Justificativa</td>
    <td></td>
  </tr>
  <tr>
    <td>Origem do Requisito</td>
    <td><a href="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md">Especificação suplementar</a> e <a href="#">requisitos elicitados</a></td>
  </tr>
  <tr>
    <td>Dependências</td>
    <td></td>
  </tr>
  <tr>
    <td>Prioridade</td>
    <td></td>
  </tr>
  <tr>
    <td>Conflitos</td>
    <td></td>
  </tr>
  <tr>
    <td>História</td>
    <td>23/11/2024</td>
  </tr>
</table>

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div>

## Conclusão

A aplicação do NFR Framework ao ChefIndica permitiu estruturar os requisitos não funcionais (RNFs) de maneira compreensível e rastreável. A análise e propagação de impactos no SIG destacam a interdependência dos softgoals e possibilitam a identificação de compromissos (trade-offs) necessários para alcançar objetivos conflitantes. Com base nos RNFs elicitados no modelo FURPS+, é possível garantir um sistema de alta qualidade que combina desempenho, confiabilidade e usabilidade, atendendo às necessidades dos usuários e ao propósito do aplicativo. O NFR Framework se mostrou uma ferramenta essencial para balancear esses atributos, fundamentando decisões de design e desenvolvimento.

## Bibliografia

> CHUNG, Lawrence; NIXON, Brian A.; YU, Eric; MYLOPOULOS, John. Non-Functional Requirements in Software Engineering. Boston: Springer, 2000.

> NIELSEN, Jakob. Usability Engineering. San Francisco: Morgan Kaufmann, 1994.

> PRESSMAN, Roger S.; MAXIM, Bruce R. Engenharia de software. 9th ed. Porto Alegre: AMGH, 2021. E-book. ISBN 9786558040118. Disponível em: https://integrada.minhabiblioteca.com.br/reader/books/9786558040118/. Acesso em: 20 nov. 2024.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |20/11/2024| NRF-Framework introdução | [Lucas Víctor](https://github.com/Lucas13032003 ) |[Zenilda Vieira](https://github.com/zenildavieira)  | 
| `1.1`  |23/11/2024| Complemento da Introdução, Metodologia e inclusão dos NFR03 e NFR04 |[Zenilda Vieira](https://github.com/zenildavieira)  |  | 
