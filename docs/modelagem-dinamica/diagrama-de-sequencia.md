# Diagrama de Sequência

## Introdução

Segundo a IBM, um diagrama de seqüência é um diagrama Unified Modeling Language (UML) que ilustra a seqüência das mensagens entre objetos em uma interação.<br>Ele descreve o intercâmbio de mensagens entre os participantes do sistema e destaca a ordem em que essas mensagens são trocadas.<br>Um diagrama de seqüência consiste em um grupo de objetos representados por linhas de vida e as mensagens que eles trocam durante a interação. [1]


## Metodologia
Combinamos alguns métodos e classes criados no diagrama de classes anteriormente e buscamos o site oficial da UML para entender os conceitos e aplicar ao nosso diagrama de sequências.

Fizemos uma abordagem geral a princípio, mas, em seguida, separamos os diferentes fluxos de modo que ficasse mais claro o funcionamento da aplicação.

Para isso, adotamos a seguinte notação:

<div align="center">
    <font size="3">
        <p style="text-align: center"><b>Tabela 1:</b> Notação do diagrama de sequência</p>
    </font>
    <table>
        <tr>
            <th style="padding: 10px; text-align: left;">Nome</th>
            <th style="padding: 10px; text-align: left;">Ícone</th>
        </tr>
        <tr>
            <td><b>Representação de classe</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqRepresentacao-de-classe.png" alt="representacao-classe">
            </td>
        </tr>
        <tr>
            <td><b>Ator</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqAtor.png" alt="ator">
            </td>
        </tr>
        <tr>
            <td><b>Caixa de ativação</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqCaixa-de-ativacao.png" alt="caixa-ativacao">
            </td>
        </tr>
        <tr>
            <td><b>Linha de ativação</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqLinha-de-ativacao.png" alt="linha-ativacao">
            </td>
        </tr>
        <tr>
            <td><b>Cenário alternativo</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqCenario-alternativo.png" alt="cenario-alternativo">
            </td>
        </tr>
        <tr>
            <td><b>Cenário optativo</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqCenario-optativo.png" alt="cenario-optativo">
            </td>
        </tr>
        <tr>
            <td><b>Referência a outro artefato</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqReferencia.png" alt="referencia">
            </td>
        </tr>
        <tr>
            <td><b>Mensagem síncrona</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqMensagem-sincrona.png" alt="mensagem-sincrona">
            </td>
        </tr>
        <tr>
            <td><b>Mensagem assíncrona</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqMensagem-assincrona.png" alt="mensagem-assincrona">
            </td>
        </tr>
        <tr>
            <td><b>Resposta de mensagem</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqResposta-da-mensagem.png" alt="resposta-mensagem">
            </td>
        </tr>
        <tr>
            <td><b>Destruição de objeto</b></td>
            <td>
            <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqDestruicao.png" alt="destruicao">           
            </td>
        </tr>
    </table>

    
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/VieiraLaris">Larissa Vieira</a>, <a href="https://github.com/cqcoding">Cecília Quaresma</a> e <a href="https://github.com/Caiomesvie">Caio Mesquita</a>,  2024.</p></font>
</div>

## Diagrama de Sequência

<center>
<p style="text-align: center"><b>Figura 1:</b> Diagrama de Sequência</p>
<div align="center">
<img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/diagrama-de-seq.png" alt="Diagrama de Sequência" >
</div>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/cqcoding">Cecília Quaresma</a>, <a href="https://github.com/VieiraLaris">Larissa Vieira</a> e <a href="https://github.com/Caiomesvie">Caio Mesquita</a>,  2024.</p></font>
</center>

## Referências Bibliográficas

> [1] IBM. Diagramas de Seqüência. IBM, 2021. Disponível em: https://www.ibm.com/docs/pt-br/rsm/7.5.0?topic=diagrams-lifelines-in-uml. Acesso em: 21 de novembro de 2024.

## Bibliografia
> UML Diagrams. UML Sequence Diagrams. Disponível em: https://www.uml-diagrams.org/sequence-diagrams.html. Acesso em: 21 de novembro de 2024.
>
> Grupo 08: UnBreja-2024.1. Modelagem: Diagrama de Sequência. Disponível em: https://unbarqdsw2024-1.github.io/2024.1_G8_UnBreja/#/Modelagem/2.1.2.1.DiagramaSequencia. Acesso em: 21 de novembro de 2024.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |21/11/2024| Criação do documento | [Cecília Quaresma](https://github.com/cqcoding) |[Larissa Vieira](https://github.com/VieiraLaris) e [Caio Mesquita](https://github.com/Caiomesvie) |
| `1.1`  |24/11/2024| Adição do diagrama de sequência | [Cecília Quaresma](https://github.com/cqcoding) |[Larissa Vieira](https://github.com/VieiraLaris) e [Caio Mesquita](https://github.com/Caiomesvie) |
| `1.2`  |25/11/2024| Adição da tabela de notações | [Larissa Vieira](https://github.com/VieiraLaris) |[Cecília Quaresma](https://github.com/cqcoding) e [Caio Mesquita](https://github.com/Caiomesvie) |
| `1.3`  |26/11/2024| Correção dos caminhos das imagens | [Larissa Vieira](https://github.com/VieiraLaris) |[Cecília Quaresma](https://github.com/cqcoding) |
| `1.4`  |26/11/2024| Correção das referências bibliográficas | [Larissa Vieira](https://github.com/VieiraLaris) |[Cecília Quaresma](https://github.com/cqcoding) |