# Diagrama de Pacotes

## Introdução

O Diagrama de Pacotes é um dos diagramas estruturais da UML (Unified Modeling Language), utilizado para organizar e visualizar a estrutura modular de sistemas complexos. Ele representa como o software é dividido em pacotes (ou módulos), ilustrando as relações de dependência entre eles. Esses pacotes podem conter classes, interfaces, ou até outros pacotes, ajudando a organizar o sistema em componentes lógicos e de fácil manutenção.

## Metodologia

Para a criação do nosso diagrama de pacotes, iniciamos com um package principal representando a aplicação ChefIndica, que contém os subpackages de backend e frontend. Esses dois pacotes interagem diretamente com o package de Testes, responsável por centralizar as validações do sistema. Cada pacote foi organizado com divisões específicas, de acordo com sua funcionalidade dentro da arquitetura do projeto, conforme descrito abaixo:

### Frontend

O pacote frontend contém toda a estrutura responsável pela interface com o usuário, dividida em subpastas para melhor organização e modularidade do código:

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

Na figura 1, é possível ver o Diagrama de Pacotes criado pela equipe.


<center>
<p style="text-align: center"><b>Figura 1:</b> Diagrama de Pacotes</p>
<div align="center">
  <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/diagrama_pacotes.png" alt="Diagrama de Pacotes" >
</div>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/izabellaalves">Izabella Alves</a>, <a href="https://github.com/PedroSampaioDias">Pedro Sampaio</a>, <a href="https://github.com/lucasqueiroz23">Lucas Queiroz</a> e <a href="https://github.com/GuilhermeB12">Guilherme Brito</a>, 2024.</p></font>
</center>


## Bibliografia
>
> BOOCH, Grady; RUMBAUGH, James; JACOBSON, Ivar. UML Guia do Usuário. 2. ed. Rio de Janeiro: Elsevier, 2006.
>

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |15/11/2024| Adiciona diagrama de pacotes | [Izabella Alves](https://github.com/izabellaalves) |[Pedro Sampaio](https://github.com/PedroSampaioDias) <br> [Lucas Queiroz](https://github.com/lucasqueiroz23) <br> [Guilherme Brito](https://github.com/GuilhermeB12)|