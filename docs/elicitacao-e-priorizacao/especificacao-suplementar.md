# Especificação Suplementar

## Introdução

Este documento apresenta a **Especificação Suplementar** para o **Chefindica**, um software de indicação e avaliação de restaurantes. A Especificação Suplementar é um artefato essencial no processo de desenvolvimento de software, pois detalha os requisitos não funcionais do sistema. Esses requisitos não estão diretamente ligados às funcionalidades específicas do aplicativo, mas abordam aspectos fundamentais como desempenho, usabilidade, confiabilidade, segurança e escalabilidade.  

Esses requisitos são cruciais para garantir que o **Chefindica** ofereça uma experiência de alta qualidade aos usuários, possibilitando um acesso ágil, avaliações confiáveis e uma interface intuitiva e segura para navegação. Eles complementam os requisitos funcionais e desempenham um papel vital na satisfação dos usuários e no sucesso do sistema como um todo.

## Metodologia

A metodologia utilizada para a elaboração deste documento baseia-se no modelo **FURPS+**, uma técnica eficaz para a coleta e organização de requisitos não funcionais. **FURPS+** é um acrônimo para **Funcionalidade, Usabilidade, Confiabilidade, Desempenho e Suporte**, que são as principais categorias de requisitos consideradas neste modelo. O “+” em **FURPS+** inclui requisitos adicionais, como restrições de design, regulamentações e requisitos relacionados à documentação e suporte ao usuário.  

Este documento foi estruturado em seções que seguem as categorias do modelo **FURPS+**. Cada seção descreve em detalhes os requisitos não funcionais aplicáveis ao **Chefindica**, abordando aspectos como a experiência do usuário ao navegar pelo aplicativo, a confiabilidade nas avaliações, o desempenho do sistema em diferentes cenários e o suporte necessário para garantir sua manutenção e evolução contínua. 

Em reunião online feita pelo Discord, os participantes [Luana Medeiros](https://github.com/LuaMedeiros), [Lucas Victor](https://github.com/Lucas13032003) e [Zenilda Vieira](https://github.com/ZenildaVieira) discutiram como a técnica funcionava e definiram que seriam elicitados os requisitos não funcionais quanto a usabilidade e confiabilidade (responsável: Lucas Víctor), desempenho e suporte (responsável: Zenilda) e restrições de design e ajuda/documentação (responsável: Luana). Após a estrutura do documento ser criada, a introdução e metodologia foi elaborada pelo Lucas Victor e revisada/complementada por Zenilda. Em seguida, cada um escreveu sua parte na especificação dos requisitos, com a explicação teórica de cada um e a tabela de RNFs. 

## FURPS+

### F: Funcionalidade (Functionality)

Os requisitos funcionais foram elicitados através das técnicas descritas no documento de [Elicitação e Priorização]([docs/elicitacao-e-priorizacao/elicitacao-e-priorizacao.md](https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/elicitacao-e-priorizacao/elicitacao-e-priorizacao.md)). Eles podem ser observados no documento [Requisitos Elicitados](https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/elicitacao-e-priorizacao/requisitos-elicitados.md). Os [Casos de Uso](https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/modelagem-organizacional-ou-cdu/diagrama-de-cdu.md) também podem ser considerados como requisitos funcionais.

### U: Usabilidade (Usability)  

A usabilidade de um sistema, segundo Nielsen [1], é o atributo de qualidade que avalia a facilidade de uso de uma interface. Uma interface com boa usabilidade possibilita que os usuários realizem suas tarefas de maneira eficiente, eficaz e satisfatória, promovendo uma experiência positiva e intuitiva.  

Na **Tabela 1**, estão apresentados os **Requisitos Não Funcionais de Usabilidade** para o aplicativo **Chefindica**.  

<div align="center">  
<font size="3"><p style="text-align: center"><b>Tabela 1:</b> Requisitos de usabilidade</p></font>  
</div>  

| ID   | Descrição |  
|------|-----------|  
| RU01 | O sistema deve ser intuitivo e fácil de usar, permitindo que os usuários encontrem e avaliem restaurantes em no máximo 3 cliques após entrar na aplicação. |  
| RU02 | O sistema deve fornecer feedback visual e/ou sonoro imediato após cada ação do usuário, informando se a operação foi realizada com sucesso ou falha. |  
| RU03 | O sistema deve permitir que os usuários desfaçam ações críticas, como exclusão de avaliações, com um botão “desfazer” ou confirmação antes de concluir a ação. |  
| RU04 | O design do sistema deve ser consistente, utilizando cores, fontes, ícones e terminologia de maneira uniforme em todas as páginas e seções. |  
| RU05 | O sistema deve ser acessível, garantindo suporte a tecnologias assistivas como leitores de tela e conformidade com as diretrizes **Web Content Accessibility Guidelines (WCAG)** [2] para inclusão de usuários com necessidades especiais. |  

<div align="center">  
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>  
</div>  

### R: Confiabilidade (Reliability)

A **Confiabilidade (Reliability)** no aplicativo **Chefindica** refere-se à capacidade do sistema de operar de maneira consistente, estável e sem falhas. Em outras palavras, os usuários podem confiar que o aplicativo estará disponível e funcionando corretamente sempre que precisarem utilizá-lo. Isso é essencial para assegurar uma experiência positiva, prevenir interrupções e manter a credibilidade da plataforma.  

Na **Tabela 2**, estão apresentados os **Requisitos Não Funcionais de Confiabilidade** para o aplicativo **Chefindica**.  

<div align="center">  
<font size="3"><p style="text-align: center"><b>Tabela 2:</b> Requisitos não funcionais sobre Confiabilidade</p></font>  
</div>  

| ID   | Descrição |  
|------|-----------|  
| RE01 | O sistema deve operar de forma contínua e estável por um período mínimo de 30 dias consecutivos. Qualquer falha não planejada deve ser resolvida em até 2 horas após a detecção. |  
| RE02 | Todos os dados de avaliações e informações críticas dos usuários devem ser armazenados de maneira segura, com backups diários. A recuperação de dados em caso de falhas deve ocorrer em até 4 horas. |  
| RE03 | O sistema deve implementar um monitoramento contínuo, com alertas automáticos para a equipe técnica em caso de problemas críticos. A equipe deve estar disponível 24/7 para suporte. |  
| RE04 | Atualizações e manutenções programadas devem ocorrer fora do horário de pico e ser previamente comunicadas aos usuários. |  
| RE05 | O sistema deve ser capaz de se recuperar automaticamente de falhas críticas, como indisponibilidade de servidores, minimizando a interrupção do serviço. |  
| RE06 | Em situações de interrupções imprevistas, o sistema deve informar os usuários de forma clara sobre o problema, o andamento da solução e o tempo estimado para normalização. |  

<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, 2024</p></font>
</div >

### P: Desempenho (Performance)

O **Desempenho (Performance)** do sistema **Chefindica** está relacionado ao tempo necessário para executar ações e à agilidade com que os usuários conseguem realizar suas tarefas. Um desempenho elevado é essencial para garantir uma experiência fluida e aumentar a produtividade do usuário. Na **Tabela 3**, estão listados os **Requisitos Não Funcionais de Desempenho** para o aplicativo **Chefindica**.

**Tabela 3:** Requisitos não funcionais sobre Desempenho

| ID    | Descrição                                                                                   |
|-------|---------------------------------------------------------------------------------------------|
| PE01  | O tempo de carregamento da página inicial do aplicativo deve ser inferior a 1 segundo.      |
| PE02  | O tempo de resposta ao acessar um perfil de restaurante deve ser inferior a 500 ms.         |
| PE03  | O tempo para realizar uma busca por restaurantes ou pratos deve ser inferior a 2 segundos.  |
| PE04  | O tempo de autenticação no login deve ser inferior a 3 segundos.                            |

<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/zenildavieira">Zenilda Vieira</a>, 2024</p></font>
</div >

### S: Suporte (Supportability)



O **Suporte (Supportability)** do sistema **Chefindica** refere-se à facilidade de manutenção, monitoramento, atualização e suporte técnico do aplicativo. É fundamental garantir que o sistema possa ser facilmente adaptado a mudanças futuras e que a equipe técnica tenha ferramentas e processos adequados para garantir a sua continuidade operacional. Na **Tabela 4**, estão listados os **Requisitos Não Funcionais de Suporte** para o aplicativo **Chefindica**.

**Tabela 4:** Requisitos não funcionais sobre Suporte

| ID    | Descrição                                                                                   |
|-------|---------------------------------------------------------------------------------------------|
| SU01  | O aplicativo deve ser desenvolvido com uma arquitetura modular para facilitar a manutenção. |
| SU02  | Todas as alterações de código devem ser registradas em um sistema de controle de versão.    |
| SU03  | O sistema deve fornecer logs detalhados para monitorar erros e eventos críticos.            |
| SU04  | As atualizações do aplicativo devem ser realizadas sem impactar a experiência do usuário.   |
| SU05  | O sistema deve oferecer suporte para adicionar novos restaurantes e categorias sem necessidade de alterações no código fonte. |

<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/zenildavieira">Zenilda Vieira</a>, 2024</p></font>
</div >

### +: Restrições de Design

As **Restrições de Design** referem-se às limitações e condições específicas que devem ser seguidas no processo de criação e desenvolvimento do sistema **Chefindica**. Essas restrições abrangem aspectos técnicos, estéticos e funcionais, garantindo que o produto final atenda aos requisitos definidos e ofereça uma experiência de qualidade. Na **Tabela 5**, estão listados os **Requisitos Não Funcionais de Restrições de Design** para o aplicativo **Chefindica**.

**Tabela 5:** Requisitos não funcionais sobre Restrições de Design

| ID    | Descrição                                                                                     |
|-------|-----------------------------------------------------------------------------------------------|
| RD01  | Todo o material visual utilizado, como imagens, ícones e gráficos, deve respeitar direitos autorais e licenças aplicáveis. |
| RD02  | A interface do usuário deve ser totalmente responsiva, adaptando-se a diferentes tamanhos de tela e dispositivos, como smartphones, tablets e desktops. |
| RD03  | O design deve seguir as diretrizes de acessibilidade da **Web Content Accessibility Guidelines (WCAG)** [2], garantindo a inclusão de usuários com diferentes necessidades. |
| RD04  | Elementos visuais como cores, fontes e ícones devem seguir um padrão consistente em todo o aplicativo para criar uma experiência coesa. |

<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div >

### +: Ajuda e Documentação

A seção de **Ajuda e Documentação** no aplicativo **Chefindica** é projetada para fornecer aos usuários informações detalhadas sobre como utilizar o sistema, suas funcionalidades, e como solucionar problemas comuns. Ter uma documentação bem estruturada e acessível é essencial para garantir que os usuários possam aproveitar ao máximo as funcionalidades do aplicativo e resolver dúvidas sem dificuldades. Essa documentação deve ser clara, precisa, e fácil de navegar.

Na **Tabela 6**, estão listados os **Requisitos Não Funcionais de Ajuda e Documentação** para o aplicativo **Chefindica**.

**Tabela 6:** Requisitos não funcionais sobre Ajuda e Documentação

| ID    | Descrição                                                                                     |
|-------|-----------------------------------------------------------------------------------------------|
| AD01  | A página de ajuda deve ser acessível em menos de 3 segundos em qualquer dispositivo.          |
| AD02  | A documentação deve ser completa e precisa, cobrindo todas as funcionalidades e características relevantes do aplicativo. |
| AD03  | A documentação deve ser atualizada e revisada trimestralmente para garantir sua relevância e precisão com as versões mais recentes do aplicativo. |
| AD04  | A maioria dos usuários (pelo menos 80%) deve conseguir encontrar a informação desejada na documentação em menos de 2 minutos de navegação. |
| AD07  | A documentação deve aderir a padrões de acessibilidade, como WCAG 2.0 ou posterior, para garantir que seja utilizável por todos os usuários, incluindo aqueles com deficiências. |

<div align="center">
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/LuaMedeiros">Luana Medeiros</a>, 2024</p></font>
</div >

## Conclusão

Após a definição dos requisitos não funcionais nesse documento, foi possível usar o NFR Framework para categorizar, organizar e analisar os RNFs e identificar como esses requisitos influenciam o sistema e como podem ser satisfeitos de forma estruturada. Os resultados podem ser verificados no documento [NFR Framework](https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/nfr_framework/docs/elicitacao-e-priorizacao/nfr-framework.md).


## Referências Bibliográficas

> [1] NIELSEN, Jakob. Usability Engineering. San Francisco: Morgan Kaufmann, 1994.
> [2] WORLD WIDE WEB CONSORTIUM. WCAG 2.0: Web Content Accessibility Guidelines. Versão 2.0. World Wide Web Consortium, 2008. Disponível em: https://www.w3.org/WAI/WCAG21/quickref/. Acesso em: 20 de novembro de 2024.

## Bibliografia

> PRESSMAN, Roger S.; MAXIM, Bruce R. Engenharia de software. 9th ed. Porto Alegre: AMGH, 2021. E-book. ISBN 9786558040118. Disponível em: https://integrada.minhabiblioteca.com.br/reader/books/9786558040118/. Acesso em: 20 nov. 2024.

## Histórico de Versões

|Versão|Data|Descrição|Autor|Revisor|
|:----:|----|---------|:-----:|:-------:|
|`1.0`|20/11/2024|Criação do documento e adição dos requisitos não funcionais|[Lucas Víctor](https://github.com/Lucas13032003) <br> [Zenilda Vieira](https://github.com/zenildavieira)|[Luana Medeiros](https://github.com/LuaMedeiros)|
|`1.1`|23/11/2024|Complemento da metodologia e adição da conclusão|[Zenilda Vieira](https://github.com/zenildavieira)|[Luana Medeiros](https://github.com/LuaMedeiros)|


