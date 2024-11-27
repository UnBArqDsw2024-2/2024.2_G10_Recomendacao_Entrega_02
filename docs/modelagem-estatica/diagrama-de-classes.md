# Diagrama de Classes

## Introdução

O diagrama de classes em UML é uma ferramenta utilizada para modelar a estrutura estática de um sistema, representando classes, seus atributos, métodos e os relacionamentos entre elas. Ele mapeia os principais objetos de um sistema, mostrando como eles se conectam e interagem, de forma a estruturar as entidades e suas responsabilidades de maneira organizada. Cada classe é uma abstração de um elemento do domínio do sistema, incluindo características (atributos) e comportamentos (métodos) que descrevem suas funcionalidades.

Além das classes, o diagrama destaca os relacionamentos entre elas, como associações, agregações, composições e heranças, permitindo a visualização das dependências e conexões. Esses relacionamentos ajudam a estruturar o sistema em módulos, a identificar possíveis pontos de integração e a definir os papéis de cada entidade no contexto geral. O diagrama de classes é utilizado como base para implementação, documentação e comunicação entre os membros da equipe de desenvolvimento.

## Metodologia

O diagrama de classes foi desenvolvido de forma colaborativa. Inicialmente, identificamos as classes principais e organizamos sua estrutura de acordo com as funcionalidades previstas. A partir dessa base, foram definidos atributos e métodos que aparentavam ser necessários para cada classe. Com a progressão do desenvolvimento, as relações entre as classes foram estabelecidas, o que permitiu identificar inconsistências e elementos redundantes. Esse processo resultou na remoção de classes, atributos e métodos desnecessários, culminando no diagrama final.

O modelo final possui uma estrutura clara, com as seguintes classes principais:

- Usuário: Concentra informações relacionadas ao indivíduo e suas interações, como histórico de avaliações.
- Restaurante: Agrega dados relacionadas aos estabelecimentos.
- Avaliação: Representa as interações entre usuários e restaurantes, armazenando informações específicas das avaliações realizadas.
- Categoria: Organiza os tipos de classificação de restaurantes utilizando uma estrutura enumerada.

## Composição das classes

O diagrama de classes padrão é composto de três partes:

- Parte superior: contém o nome da classe.
- Parte do meio: contém os atributos da classe.
- Parte inferior: inclui as operações da classe (métodos)

<div align = "center"><img src="https://raw.githubusercontent.com/UnBArqDsw2023-2/2023.2_G8_ProjetoMagazineLuiza/main/docs/Assets/diagrama_cla_exe.png" alt="Figura 1: Diagrama de Classes exemplo." height="300" width="350">
<p>Figura 1: Exemplo de classe. Fonte: Projeto Magazine Luiza, Grupo 8, 2023</p></div>

## Diagrama de Classes

<center>
<p style="text-align: center"><b>Figura 1:</b> Diagrama de Classes</p>
<div align="center">
<img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/diagrama_classes.png" alt="Diagrama de Classes" >
</div>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/izabellaalves">Izabella Alves</a>, <a href="https://github.com/PedroSampaioDias">Pedro Sampaio</a>, <a href="https://github.com/lucasqueiroz23">Lucas Queiroz</a>, <a href="https://github.com/VieiraLaris">Larissa Vieira</a> e <a href="https://github.com/cqcoding">Cecília Quaresma</a>,  2024.</p></font>
</center>

## Legenda

Por padrão utilizamos os seguintes elementos em nosso diagrama:

<div align = "center"><img src="https://github.com/UnBArqDsw2023-1/2023.1_G2_ProjetoMercadoLivre/blob/main/docs/Assets/diagramas/legenda_diagrama_de_classes.png?raw=true" alt="Figura 3: Diagrama de Classes Legenda." height="500" width="450">
<p>Figura 3: Legenda Diagrama de Classes. Fonte: Projeto Mercado Livre, Grupo 2, 2023</p></div>

## Referências Bibliográficas

> Orientações básicas na elaboração de um diagrama de classes. Disponível em: https://www.devmedia.com.br/orientacoes-basicas-na-elaboracao-de-um-diagrama-de-classes/37224. Acesso em: 16 de nov. 2024.

> O que é um diagrama de classe UML. Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-classe-uml. Acesso em: 16 de nov. 2024.

> Diagramas de Classes. Disponível em: https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=structure-class-diagrams. Acesso em: 16 de nov. 2024.

> Modelo de Diagrama de Classe UML. Disponível em: https://miro.com/pt/modelos/diagrama-classe-uml. Acesso em: 16 de nov. 2024.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  | 16/11/2024 | Adição do diagrama de classes | [Pedro Sampaio](https://github.com/PedroSampaioDias) | [Cecília Quaresma](https://github.com/cqcoding) |
| `1.1`  | 23/11/2024 | Adição legenda e composição | [Mateus Fidelis](https://github.com/MatsFidelis) | [Lucas Queiroz](https://github.com/lucasqueiroz23) |
| `1.2`  | 25/11/2024 | Correção das datas de acesso | [Pedro Sampaio](https://github.com/PedroSampaioDias) | [Cecília Quaresma](https://github.com/cqcoding) |
