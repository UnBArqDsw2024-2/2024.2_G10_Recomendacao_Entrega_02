# Diagrama de Sequência

## Introdução

Segundo a IBM [1], um diagrama de sequência é um diagrama da Unified Modeling Language (UML) que ilustra a sequência de mensagens trocadas entre objetos em uma interação. Ele descreve o intercâmbio de mensagens entre os participantes do sistema, destacando a ordem em que essas mensagens são enviadas. Este artefato é composto por um grupo de objetos representados por linhas de vida e pelas mensagens que esses objetos trocam durante a interação.

De acordo com a plataforma Lucidchart [2], o uso de diagramas de sequência oferece diversos benefícios, como:
* Representar os detalhes de um caso de uso UML.
* Modelar a lógica de um processo, função ou operação sofisticado.
* Ver como objetos e componentes interagem uns com os outros para concluir um processo.
* Planejar e compreender a funcionalidade detalhada de um cenário existente ou futuro.


## Metodologia
Para modelar o diagrama de sequência, combinamos métodos e classes previamente definidos no [diagrama de classes](https://unbarqdsw2024-2.github.io/2024.2_G10_Recomendacao_Entrega_02/#/modelagem-estatica/diagrama-de-classes). Após realizar uma pesquisa no site oficial da UML para compreender os conceitos e aplicá-los ao nosso artefato, elaboramos o diagrama utilizando a plataforma Miro.

Inicialmente, adotamos uma abordagem geral, mas posteriormente segmentamos os diferentes fluxos para tornar o funcionamento da aplicação mais claro e organizado.

Utilizamos a seguinte notação para representar os elementos do diagrama:

<div align="center">
    <font size="3">
        <p style="text-align: center"><b>Tabela 1:</b> Notação do diagrama de sequência</p>
    </font>
    <table>
        <tr>
            <th style="padding: 10px; text-align: left;">Nome</th>
            <th style="padding: 10px; text-align: left;">Ícone</th>
            <th style="padding: 10px; text-align: left;">Função</th>
        </tr>
        <tr>
            <td><b>Representação de classe</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqRepresentacao-de-classe.png" alt="representacao-classe">
            </td>
            <td> Simboliza uma classe do sistema ou da interação.</td>
        </tr>
        <tr>
            <td><b>Ator</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqAtor.png" alt="ator">
            </td>
            <td> Entidade externa (como um usuário) que interage com o sistema.</td>
        </tr>
        <tr>
            <td><b>Caixa de ativação</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqCaixa-de-ativacao.png" alt="caixa-ativacao">
            </td>
            <td> Período em que o objeto está ativo, executando uma operação ou aguardando uma resposta.</td>
        </tr>
        <tr>
            <td><b>Linha de ativação</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqLinha-de-ativacao.png" alt="linha-ativacao">
            </td>
            <td> Tempo de existência do objeto. </td>
        </tr>
        <tr>
            <td><b>Cenário alternativo</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqCenario-alternativo.png" alt="cenario-alternativo">
            </td>
            <td> Descreve fluxos de interação em que há mais de uma alternativa de execução, dependendo de condições específicas. </td>
        </tr>
        <tr>
            <td><b>Cenário optativo</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqCenario-optativo.png" alt="cenario-optativo">
            </td>
            <td> Descreve cenários que não são obrigatórios no fluxo principal. </td>
        </tr>
        <tr>
            <td><b>Referência a outro artefato</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqReferencia.png" alt="referencia">
            </td>
            <td> Simboliza um cenário ou fluxo de outro artefato que está sendo referenciado. </td>
        </tr>
        <tr>
            <td><b>Mensagem síncrona</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqMensagem-sincrona.png" alt="mensagem-sincrona">
            </td>
            <td> Indica que emissor aguarda uma resposta antes de prosseguir. </td>
        </tr>
        <tr>
            <td><b>Mensagem assíncrona</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqMensagem-assincrona.png" alt="mensagem-assincrona">
            </td>
            <td> Indica que emissor não aguarda uma resposta imediata e pode continuar com outros processamentos. </td>
        </tr>
        <tr>
            <td><b>Resposta de mensagem</b></td>
            <td>
                <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqResposta-da-mensagem.png" alt="resposta-mensagem">
            </td>
            <td> Retorno de uma função previamente acionada. </td>
        </tr>
        <tr>
            <td><b>Destruição de objeto</b></td>
            <td>
            <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/seqDestruicao.png" alt="destruicao">           
            </td>
            <td> Simboliza que o objeto foi destruído ou deixou de existir. </td>
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
>
> [2] Lucidchart. O que é um diagrama de sequência UML?. Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml. Acesso em: 29 de novembro de 2024.

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
| `1.5`  |29/11/2024| Adição da coluna "Função" na tabela de notações e melhora nos textos | [Larissa Vieira](https://github.com/VieiraLaris) |[Cecília Quaresma](https://github.com/cqcoding) e [Caio Mesquita](https://github.com/Caiomesvie) |