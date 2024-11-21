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

## XXX
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
