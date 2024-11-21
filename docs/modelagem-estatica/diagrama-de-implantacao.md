# Diagrama de Implantação

## Introdução
O diagrama de implantação é uma ferramenta usada para representar como os componentes de um sistema de software são distribuídos fisicamente em dispositivos de hardware, como servidores, computadores e outros dispositivos conectados. Ele mostra, de forma clara e visual, onde cada parte do sistema será executada e como essas partes se comunicam entre si.

Esse tipo de diagrama é especialmente útil para entender e planejar a infraestrutura necessária para o funcionamento do sistema, ajudando a garantir que os recursos de hardware sejam suficientes para suportar o software. Além disso, ele auxilia no planejamento da escalabilidade, na identificação de potenciais gargalos e na comunicação entre as equipes de desenvolvimento e infraestrutura. Com uma linguagem simples e direta, o diagrama de implantação ajuda a conectar as decisões de arquitetura de software ao ambiente físico onde o sistema será implementado, garantindo que o projeto seja eficiente e sustentável.

## Metodologia
**Metodologia para o Diagrama de Implantação**  

Para o desenvolvimento do Diagrama de Implantação, foi analisada a estrutura do sistema, considerando a distribuição dos componentes físicos e a comunicação entre eles. O objetivo foi representar de forma clara como o sistema funciona no ambiente de hardware, destacando as interações entre os dispositivos.  

A equipe utilizou a ferramenta Lucidchart para a criação do diagrama, aproveitando seus recursos de colaboração em tempo real para facilitar o trabalho em conjunto.  

Os membros da equipe ([Caio Mesquita](https://github.com/Caiomesvie), [Guilherme Brito](https://github.com/GuilhermeB12), [Zenilda Vieira](https://github.com/zenildavieira) e [Luana Medeiros](https://github.com/LuaMedeiros)) realizaram estudos prévios sobre diagramas de implantação e trocaram ideias durante uma reunião no Discord, onde discutiram o material pesquisado e trabalharam coletivamente na elaboração do diagrama.  

No modelo gerado, o fluxo foi representado da seguinte forma: o acesso ao sistema é iniciado por um dispositivo do usuário (desktop), que se conecta a um firewall para garantir a segurança da rede. Após essa etapa, a comunicação segue para um servidor web, que repassa as solicitações ao servidor de aplicação. Por fim, o servidor de aplicação acessa o banco de dados para processar as informações necessárias.

## Diagrama de Implantação

Na figura 1, abaixo, está o diagrama de implantação.

<div align="center">
    <font size="3">
        <p style="text-align: center"><b>Figura 1:</b> Diagrama de Implantação</p>
    </font>

<img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/diagrama_implantacao.png" alt="Diagrama da Implantação" width="70%">

<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Caiomesvie">Caio Mesquita</a>, <a href="https://github.com/GuilhermeB12"> Guilherme Brito </a> e <a href="https://github.com/zenildavieira"> Zenilda Vieira </a>, 2024</p></font>
</div>

## Bibliografia
1. Tutorial do Diagrama de Implantação. Disponível em: <https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-implantacao/>. Acesso em: 20 nov. 2024.
2. Rational Software Architect Standard Edition 7.5.5. Disponível em: <https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams>. Acesso em: 20 nov. 2024.

## Referências Bibliográficas
1. O que é um diagrama de implementação? Disponível em: <https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml>. Acesso em: 20 nov. 2024.
2. PAIVA. Curso de UML - diagrama de implantação. Disponível em: <https://www.youtube.com/watch?v=DgERD0HgggQ>. Acesso em: 20 nov. 2024.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |18/11/2024| Adição da introdução | [Luana Medeiros](https://github.com/LuaMedeiros) |[Zenilda Vieira](https://github.com/zenildavieira) |
| `1.1`  |20/11/2024| Adição do Diagrama de implantação | [Caio Mesquita](https://github.com/Caiomesvie)<br>[Guilherme Brito](https://github.com/GuilhermeB12)<br>[Zenilda Vieira](https://github.com/zenildavieira)| [Luana Medeiros](https://github.com/LuaMedeiros) |
| `1.2`  |20/11/2024| Adição da metodologia | [Luana Medeiros](https://github.com/LuaMedeiros) | |
