# Diagrama de Pacotes

## Introdução

<p style="text-align: justify; text-indent: 2em;"> O Diagrama de Pacotes é um dos diagramas estruturais da UML (Unified Modeling Language), utilizado para organizar e visualizar a estrutura modular de sistemas complexos. Ele representa como o software é dividido em pacotes (ou módulos), ilustrando as relações de dependência entre eles. Esses pacotes podem conter classes, interfaces, ou até outros pacotes, ajudando a organizar o sistema em componentes lógicos e de fácil manutenção. </p>

## Metodologia

<p style="text-align: justify; text-indent: 2em;"> Para a criação do nosso diagrama de pacotes, iniciamos com um package principal representando a aplicação ChefIndica, que contém os subpackages de backend e frontend. Esses dois pacotes interagem diretamente com o package de Testes, responsável por centralizar as validações do sistema. Cada pacote foi organizado com divisões específicas, de acordo com sua funcionalidade dentro da arquitetura do projeto e a equipe escolheu utilizar o Service Repository Pattern como uma das principais formas de organização do projeto. </p>

<p style="text-align: justify; text-indent: 2em;"> O Service Repository Pattern é amplamente utilizado no desenvolvimento orientado por domínio (Domain-Driven Design - DDD) para organizar e modularizar o acesso e a lógica de negócios de sistemas complexos. O padrão de repositório (Repository) abstrai o acesso aos dados, atuando como uma coleção em memória que encapsula a lógica de persistência. Ele permite que operações como adicionar, remover e consultar objetos sejam realizadas sem expor detalhes da camada de mapeamento de dados. Já o padrão de serviço (Service) encapsula regras de negócios que não se encaixam diretamente em um objeto de domínio, operando como objetos sem estado que facilitam a execução de lógica específica. </p>

<p style="text-align: justify; text-indent: 2em;"> Esses dois padrões, quando usados em conjunto, promovem a separação de responsabilidades, reduzem duplicações no código e organizam de forma mais clara os diferentes aspectos de um sistema. Martin Fowler, em Patterns of Enterprise Application Architecture [1], destaca a importância do padrão de repositório para mediar entre o domínio e a camada de mapeamento de dados, provendo uma interface consistente para acessar objetos de domínio.</p>

### Frontend

<p style="text-align: justify; text-indent: 2em;"> O pacote frontend contém toda a estrutura responsável pela interface com o usuário, dividida em subpastas para melhor organização e modularidade do código: </p>

- **Utils**: Contém funções utilitárias reutilizáveis, como formatação de dados e cálculos.
- **Components**: Reúne os componentes reutilizáveis da interface, como botões, cabeçalhos e rodapés.
- **Pages**: Armazena as páginas principais do sistema.
- **Contexts**: Gerencia o estado global da aplicação utilizando o contexto do React.
- **Assets**: Contém arquivos estáticos, como imagens, ícones e estilos CSS.
- **Services**: Gerencia as interações entre os componentes criados e os dados vindos dos repositories.
- **Repositories**: Define as chamadas para APIs.

### Backend
- **Utils**: Contém funções utilitárias reutilizáveis, como formatação de dados e cálculos.
- **Services**: Centraliza a lógica de negócios e as operações mais complexas que envolvem diferentes camadas.
- **Repositories**: Responsável por acessar e manipular os dados no banco de dados.
- **Models**: Define as estruturas de dados, como entidades e suas relações.
- **Exceptions**: Contém classes para lidar com exceções personalizadas, facilitando a tratativa de erros.
- **Interfaces**: Define contratos e abstrações, promovendo a flexibilidade e padronização na implementação de funcionalidades.

## Diagrama de Pacotes

<p style="text-align: justify; text-indent: 2em;"> Na Figura 1, é apresentado o diagrama de pacotes em alto nível elaborado pela equipe, destacando a relação entre os pacotes backend e frontend. Já as Figuras 2 e 3 exploram em maior profundidade, detalhando como esses grandes componentes são subdivididos em seus respectivos subcomponentes.</p>

<center>
<p style="text-align: center"><b>Figura 1:</b> Diagrama de pacotes em alto nível</p>
<div align="center">
  <img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/diagrama_pacotes_alto_nivel.png?raw=true" alt="Diagrama de pacotes em alto nível" >
</div>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/izabellaalves">Izabella Alves</a>, <a href="https://github.com/PedroSampaioDias">Pedro Sampaio</a>, <a href="https://github.com/lucasqueiroz23">Lucas Queiroz</a> e <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, 2024.</p></font>
</center>

<center>
<p style="text-align: center"><b>Figura 2:</b> Diagrama de pacotes do backend</p>
<div align="center">
  <img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/diagrama_pacotes_backend.png?raw=true" alt="Diagrama de pacotes do backend" >
</div>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/izabellaalves">Izabella Alves</a>, <a href="https://github.com/PedroSampaioDias">Pedro Sampaio</a>, <a href="https://github.com/lucasqueiroz23">Lucas Queiroz</a> e <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, 2024.</p></font>
</center>

<center>
<p style="text-align: center"><b>Figura 3:</b> Diagrama de pacotes do frontend</p>
<div align="center">
  <img src="https://github.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/blob/main/docs/imagens/diagrama_pacotes_frontend.png?raw=true" alt="Diagrama de pacotes do frontend" >
</div>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/izabellaalves">Izabella Alves</a>, <a href="https://github.com/PedroSampaioDias">Pedro Sampaio</a>, <a href="https://github.com/lucasqueiroz23">Lucas Queiroz</a> e <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, 2024.</p></font>
</center>

## Referências Bibliográficas

>
> [1] FOWLER, Martin. Patterns of Enterprise Application Architecture. Boston: Addison-Wesley, 2003. Disponível em: https://martinfowler.com/eaaCatalog/repository.html. Acesso em: 15 nov. 2024.
>

## Bibliografia
>
> BOOCH, Grady; RUMBAUGH, James; JACOBSON, Ivar. UML Guia do Usuário. 2. ed. Rio de Janeiro: Elsevier, 2006.
>
> THE UNIFIED MODELING LANGUAGE. UML Package Diagrams Overview. Disponível em: https://www.uml-diagrams.org/package-diagrams-overview.html. Acesso em: 15 nov. 2024.
>

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |15/11/2024| Adiciona diagrama de pacotes | [Izabella Alves](https://github.com/izabellaalves) |[Pedro Sampaio](https://github.com/PedroSampaioDias) <br> [Lucas Queiroz](https://github.com/lucasqueiroz23) <br> [Guilherme Brito](https://github.com/GuilhermeB12)|
| `1.1`  |25/11/2024| Melhora na organização das imagens | [Pedro Sampaio](https://github.com/PedroSampaioDias) |[Izabella Alves](https://github.com/izabellaalves) <br> [Lucas Queiroz](https://github.com/lucasqueiroz23) <br> [Guilherme Brito](https://github.com/GuilhermeB12)|
| `1.2`  |29/11/2024| Descrevendo melhor a introdução | [Júlia Yoshida](https://github.com/juliaryoshida) |[Mateus Fidelis](https://github.com/MatsFidelis)|
