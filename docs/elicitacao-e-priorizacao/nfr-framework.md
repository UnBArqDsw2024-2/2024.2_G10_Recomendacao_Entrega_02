# NFR Framework
### Introdução   

O **NFR (Non-Functional Requirements) Framework**, ou *Framework de Requisitos Não Funcionais*, é uma abordagem essencial no desenvolvimento de software e engenharia de sistemas. No contexto do *Chefindica*—um software de indicação e avaliação de restaurantes—este framework ajuda a definir e gerenciar requisitos que não estão diretamente ligados às funcionalidades específicas do sistema (como a busca ou cadastro de restaurantes), mas sim às características que impactam a qualidade geral do software. Entre essas características estão o desempenho, a segurança, a usabilidade e a experiência do usuário, elementos críticos para o sucesso do *Chefindica*.  

Esses requisitos não funcionais (NFRs) desempenham um papel essencial ao determinar como o sistema deve se comportar para oferecer uma experiência eficiente, confiável e agradável para os usuários, garantindo, por exemplo, tempos de resposta rápidos ao buscar restaurantes, proteção de dados pessoais ao avaliar estabelecimentos e interfaces intuitivas para navegação.

O NFR Framework utiliza o conceito de "softgoal", que se refere a um objetivo que não possui critérios de satisfação estritamente definidos. No *Chefindica*, os softgoals podem estar conectados, refletindo como um requisito, como "segurança de dados", influencia outro, como "confidencialidade das avaliações".  

O **NFR Framework** organiza essas conexões em gráficos chamados *Softgoal Interdependency Graphs (SIGs)*. Esses gráficos registram as considerações dos desenvolvedores sobre os softgoals e suas interdependências. No caso do *Chefindica*, os SIGs podem detalhar decisões sobre requisitos como: 

- **Tempo de Resposta**: O sistema deve retornar sugestões de restaurantes em menos de 2 segundos.  
- **Privacidade do Usuário**: Garantir que as avaliações sejam armazenadas de forma anônima.  
- **Acessibilidade**: Tornar o sistema acessível para usuários com deficiência visual.  

O SIG também ajuda a justificar as escolhas feitas durante o desenvolvimento, facilitando a avaliação de alto nível para garantir que os requisitos não funcionais sejam atendidos.

### Tipos de Softgoals 

Os softgoals no NFR Framework se dividem em três categorias principais, que são representadas no gráfico de interdependência. Esses softgoals são adaptados para o *Chefindica* da seguinte forma:  

1. **Softgoals NFR**:  
   Representam os requisitos não funcionais principais do sistema.  
   - Exemplo no *Chefindica*: "Garantir baixa latência no carregamento da página inicial".  

2. **Softgoals de Operacionalização**:  
   Correspondem às soluções de implementação para alcançar os softgoals NFR ou outros softgoals de operacionalização.  
   - Exemplo no *Chefindica*: "Implementar cache local para reduzir o tempo de busca de restaurantes".  

3. **Softgoals de Afirmação**:  
   Levam em conta as características do domínio, como prioridades do sistema ou comportamento dos usuários.  
   - Exemplo no *Chefindica*: "Priorizar a segurança dos dados dos usuários em detrimento de algumas otimizações de desempenho".  

A **Figura 1** abaixo ilustra a representação dos tipos de softgoals, que pode ser utilizada como legenda para os gráficos SIGs do *Chefindica*.  

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 1:</b> Representação dos tipos de softgoal adaptados para o *Chefindica*.</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/imagens/nfr-softgoals.png?raw=true" style="width: 45%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> (CHUNG et al., 2000).</a></p></font>
</div>

### Avaliação e Propagação de Impactos  

No NFR Framework, a avaliação verifica se os requisitos não funcionais foram atendidos. Isso ocorre por meio da atribuição de rótulos aos softgoals no SIG. No *Chefindica*, o processo de avaliação pode verificar, por exemplo:  

- O tempo médio de resposta atende aos 2 segundos especificados?  
- A implementação de criptografia garante a privacidade dos dados?  
- A interface de acessibilidade permite o uso por pessoas com deficiência?  

Os rótulos possíveis incluem:  
- **Satisfeito**: O requisito foi totalmente atendido.  
- **Parcialmente Satisfeito**: Foi atendido em parte, mas há margem para melhorias.  
- **Não Atendido**: O requisito não foi alcançado.  
- **Parcialmente Não Atendido**: O requisito foi comprometido de forma significativa.  
- **Conflitante**: Existem conflitos entre requisitos.  
- **Indeterminado**: Ainda não foi avaliado ou não possui informações suficientes.  

A **Figura 2** apresenta os rótulos de propagação de impactos que podem ser usados no SIG do *Chefindica*.  

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 2:</b> Rótulos de propagação de impactos adaptados ao *Chefindica*.</p></font>

<img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/imagens/nfr-impactos.png?raw=true" style="width: 65%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> (CHUNG et al., 2000).</a></p></font>
</div>

Com base nesses rótulos, é possível ajustar as prioridades e refinar a implementação para garantir que o *Chefindica* atenda às expectativas dos usuários e aos objetivos de qualidade definidos pelo NFR Framework.

## Metodologia

Neste documento, serão apresentads 6 NFRs, que foram definidos a partir do nosso documento de [Especificação Suplementar](https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md), que por sua vez se baseou no modelo FURPS+.

Para cada categoria, foi feito um SIG (Softgoal Interdependency Graph), um diagrama da propagação de impactos e um cartão de especificação, que possui informações sobre o NFR, como a descrição, a categoria, os conflitos, a origem, os critérios e outras informações.

## NFR Framework


### NFR01 - Usabilidade 

Usabilidade, segundo Nielsen, é a medida de quão fácil e agradável é usar um sistema para alcançar os objetivos dos usuários.


#### Softgoal Interdependency Graph

O Softgoal Interdependency Grap do softgoal "Usabilidade" pode ser visto na figura 3.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 3:</b> Softgoal Interdependency Grap do softgoal "Usabilidade".</p></font>

<img src="https://github.com/Requisitos-de-Software/2023.2-Economia-DF/blob/main/docs/imagens/diagramausabilidade.png?raw=true" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>

#### Propagação de Impactos

A propagação de impactos do softgoal "Usabilidade" pode ser visto na figura 4.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 4:</b> Propagação de impactos do softgoal "Usabilidade"</p></font>

<img src="https://github.com/Requisitos-de-Software/2023.2-Economia-DF/blob/main/docs/imagens/propagacaousabilidade.drawio.png?raw=true" style="width: 85%;">

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
    <td>O requisito "Usabilidade" refere-se à capacidade do sistema de entregar uma boa usabilidade para os usuários do aplicativo do "Economia DF".</td>
  </tr>
  <tr>
    <td>Justificativa</td>
    <td>Uma boa Usabilidade é fundamental para garantir que os usuários possam utilizar o aplicativo com eficiência e garantir uma satisfação do usuário, aumentando a acessibilidade e por consequência tendo uma redução de erros.</td>
  </tr>
  <tr>
    <td>Origem do Requisito</td>
    <td><a href="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/especificacao-suplementar.md">Especificação suplementar</a> e <a href="#">requisitos elicitados</a></td>
  </tr>
  <tr>
    <td>Dependências</td>
    <td>Não foram identificadas restrições ou dependências específicas, mas a atualização da documentação deve ser planejada e coordenada com as versões do aplicativo.</td>
  </tr>
  <tr>
    <td>Prioridade</td>
    <td>O requisito de "Usabilidade" é de alta prioridade, uma vez que influencia diretamente a satisfação do usuário e a eficácia do aplicativo.</td>
  </tr>
  <tr>
    <td>Conflitos</td>
    <td>Não foi identificado nenhum conflito.</td>
  </tr>
  <tr>
    <td>História</td>
    <td>04/11/2024</td>
  </tr>
</table>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>


###  NFR02 - Confiabilidade (Reliability)
A "Confiabilidade" em um aplicativo é uma característica crucial que se refere à capacidade do aplicativo de funcionar de maneira consistente, estável e sem falhas. Isso assegura que os [usuários](https://github.com/Requisitos-de-Software/2023.2-Economia-DF/blob/main/docs/modelagem/lexicos.md#objetos) possam confiar que o aplicativo estará disponível e operando corretamente sempre que precisarem utilizá-lo. A confiabilidade desempenha um papel essencial para garantir uma experiência positiva do usuário, evitando erros, interrupções inesperadas e mantendo a credibilidade do aplicativo. Como a "Ajuda e Documentação" são recursos essenciais para orientar os usuários, a confiabilidade é o alicerce que sustenta a confiança dos usuários no aplicativo, permitindo que eles utilizem as informações da "Ajuda e Documentação" com segurança e eficácia.

#### Softgoal Interdependency Graph

O Softgoal Interdependency Grap do softgoal "Confiabilidade (Reliability)" pode ser visto na figura 5.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 5:</b> Softgoal Interdependency Grap do softgoal "Confiabilidade (Reliability)".</p></font>

<img src="https://github.com/Requisitos-de-Software/2023.2-Economia-DF/blob/main/docs/imagens/NFR_Confiabilidade.png?raw=true" style="width: 85%;">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div>


#### Propagação de Impactos

A propagação de impactos do softgoal "Confiabilidade (Reliability)" pode ser visto na figura 6.

<div align="center">
<font size="3"><p style="text-align: center"><b>Figura 6:</b> Propagação de impactos do softgoal "Confiabilidade (Reliability)"</p></font>

<img src="https://github.com/Requisitos-de-Software/2023.2-Economia-DF/blob/main/docs/imagens/Propaga%C3%A7%C3%A3o_de_impactos_do_softgoal_Confiabilidade.png?raw=true" style="width: 85%;">

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



## Bibliografia

> SERRANO, Maurício;  SERRANO, Milene. Requisitos - Aula 17. Local: UnB-FGA, Gama, DF. Apresentação de Power Point. Disponível em: [Requisitos - Aula 17](https://aprender3.unb.br/pluginfile.php/2692836/mod_resource/content/1/Requisitos%20-%20Aula%20019a.pdf). Acesso em: 03 de novembro de 2023.
> 

## Referências Bibliográficas

> [1] SILVA, Reinaldo Antônio da. NFR4ES: Um Catálogo de Requisitos Não-Funcionais para Sistemas Embarcados. Universidade Federal de Pernambuco, 2019. Disponível em: <https://aprender3.unb.br/pluginfile.php/2692835/mod_resource/content/2/DISSERTA%C3%87%C3%83O%20Reinaldo%20Ant%C3%B4nio%20da%20Silva.pdf>. Acesso em: 02 de novembro de 2023.
>

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |20/11/2024| NRF-Framework introdução | [Lucas Víctor](https://github.com/Lucas13032003 ) |[xxxx](xxxx)  | 
