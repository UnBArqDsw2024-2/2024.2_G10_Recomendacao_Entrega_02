
# Diagrama de Componentes  

## 1. Introdução  
Os diagramas de componentes desempenham um papel fundamental na representação e compreensão da estrutura física de sistemas de software. Eles oferecem uma visão clara da organização dos principais módulos, bibliotecas, arquivos executáveis e outros elementos de software reutilizáveis. Esses diagramas destacam como os componentes estão interconectados, evidenciando dependências, interfaces e relações que sustentam a funcionalidade do sistema.

No contexto de projetos de software, os diagramas de componentes auxiliam na divisão do sistema em partes menores e mais gerenciáveis, permitindo uma análise mais detalhada das interações entre os elementos. Além disso, servem como ferramenta de documentação, facilitando o trabalho das equipes de desenvolvimento e manutenção, promovendo modularidade e uma visão clara das arquiteturas lógicas e físicas do sistema.

Este documento detalha o processo de construção de um diagrama de componentes para um sistema, abordando suas funcionalidades, organização e interações entre os elementos.

## 2. Metodologia  
Para elaborar o diagrama de componentes, foram seguidas as etapas descritas abaixo:

- **Identificação dos Componentes:** Os principais componentes do sistema foram definidos com base nos requisitos funcionais e técnicos.  
- **Mapeamento das Interações:** As interações e dependências entre os componentes foram analisadas, identificando conexões lógicas e interfaces entre eles.  
- **Criação do Diagrama:** Com o uso de uma ferramenta de modelagem UML, o diagrama foi desenvolvido para representar os componentes e suas conexões de forma clara e compreensível.  
- **Revisão e Validação:** Após a construção, o diagrama foi revisado por especialistas para garantir a precisão das representações e a conformidade com os objetivos do sistema.

### Tabela de Elementos do Diagrama  

| **Símbolo**             | **Descrição**                                                              |
|-------------------------|---------------------------------------------------------------------------|
| `<<subsystem>>`         | Subsistema: Representa um módulo ou uma funcionalidade específica do sistema. |
| 🟦                       | Componente: Unidade funcional ou módulo dentro do sistema.                  |
| 📄                       | Interface: Ponto de comunicação que o componente fornece ou requer.         |
| <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/solicitação_de%20interface.png" alt="Diagrama de Classes" width="60"> | Conexão de Interface: Representa a comunicação entre componentes via interfaces. |
| <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/depedencia.png" alt="Diagrama de Classes" width="60"> | Dependência: Mostra que um componente depende de outro para funcionar.      |
| <img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/refs/heads/main/docs/imagens/porta.png" alt="Diagrama de Classes" width="60">               | Porta: Indica o ponto de interação onde as interfaces são expostas.         |

## 3. Descrição  

Este diagrama apresenta os principais componentes do sistema *Chef Indica* como é possível ver na figura 1, que visa permitir que os usuários cadastrem e avaliem restaurantes, além de interagir com avaliações de outros usuários. A estrutura está organizada em subsistemas que promovem modularidade, separação de responsabilidades e interação eficiente entre os componentes.

<center>
<p style="text-align: center"><b>Figura 1:</b> Diagrama de Componentes</p>
<div align="center">
<img src="https://raw.githubusercontent.com/UnBArqDsw2024-2/2024.2_G10_Recomendacao_Entrega_02/84675e8d41664681e859326cfdfae3036a450ad0/docs/imagens/Diagrama%20de%20Componentes%20-%20ChefIndica.png" alt="Diagrama de Classes" >
</div>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/Lucas13032003">Lucas Víctor</a>, <a href="https://github.com/MatsFidelis">Mateus Fidelis</a>, <a href="https://github.com/Maliz30">Maria Alice</a> e <a href="https://github.com/juliaryoshida">Júlia Yoshida</a>, 2024.</p></font>
</center>

1. **Subsistema `<<subsystem>> Usuário`**
   - Contém os componentes que gerenciam as ações do usuário, como:
     - **Barra de Pesquisa por Restaurante:** Permite pesquisar restaurantes cadastrados.
     - **Restaurante:** Responsável por gerenciar o cadastro de novos restaurantes.
     - **Avaliação:** Permite aos usuários escrever e curtir avaliações de restaurantes.
     - **Autenticação:** Gerencia sessões e autenticação de usuários para acesso às funcionalidades.

2. **Subsistema `<<subsystem>> Banco de Dados / Restaurantes`**
   - Armazena e gerencia informações sobre os restaurantes cadastrados.
   - Contém a **Biblioteca**, que expõe as interfaces para busca e gerenciamento de dados de restaurantes.

3. **Subsistema `<<subsystem>> Banco de Dados / Avaliações`**
   - Gerencia as informações relacionadas às avaliações realizadas pelos usuários.
   - Inclui a **Biblioteca**, que fornece suporte ao gerenciamento de avaliações.

4. **Subsistema `<<subsystem>> Registro de Contas`**
   - Responsável pelo gerenciamento de usuários e seus dados.
   - Contém o componente **Usuários**, que armazena informações relacionadas às contas.

#### **Interações Principais**

1. **Cadastro e Pesquisa de Restaurantes:**
   - O usuário cadastra um restaurante através do componente **Restaurante**.
   - As informações são enviadas para o subsistema **Banco de Dados / Restaurantes**, que armazena os dados.

2. **Escrita e Curtida de Avaliações:**
   - O componente **Avaliação** recebe as interações dos usuários.
   - As informações são encaminhadas para o subsistema **Banco de Dados / Avaliações**.

3. **Autenticação e Sessão:**
   - A autenticação do usuário é gerenciada pelo componente **Autenticação**, que interage com o subsistema **Registro de Contas** para validar os dados.

4. **Conexões e Dependências:**
   - Cada subsistema expõe interfaces para comunicação, promovendo uma arquitetura modular e escalável.

## 4. Conclusão  
O diagrama de componentes é uma ferramenta essencial para compreender a estrutura física de sistemas de software. Ele promove a documentação e organização do sistema, evidenciando as conexões e dependências entre seus elementos.

A criação desse diagrama permite uma análise clara dos componentes e suas interações, sendo útil tanto para o planejamento quanto para a manutenção e evolução do sistema.

## 5. Bibliografia  
- FOWLER, M.; TORTELLO, J. *UML essencial: um breve guia para a linguagem-padrão de modelagem de objetos*. Porto Alegre: Bookman, 2005.  
- Lucidchart. *Diagrama de componentes UML: o que é, como fazer e exemplos*. Disponível em: [https://www.lucidchart.com](https://www.lucidchart.com).  
- UML-Diagrams.org. *UML Component Diagram*. Disponível em: [https://www.uml-diagrams.org](https://www.uml-diagrams.org).  

## 6. Histórico de Versões  

| **Versão** | **Data**       | **Descrição**         | **Autor(a)**                          | **Revisor(a)**                     |
|:----------:|----------------|-----------------------|---------------------------------------|------------------------------------|
| `1.0`      | 18/11/2024     | Descrição inicial     | [Mateus Fidelis](https://github.com/MatsFidelis) | [Maria Alice](https://github.com/Maliz30), [Júlia Yoshida](https://github.com/juliaryoshida) |  
| `1.1`  | 24/11/2024 | Adição  | [Lucas Víctor](https://github.com/Lucas13032003) |[Maria Alice](https://github.com/Maliz30)|
| `1.2`  | 28/11/2024| Revisão dos dados e correção de imagens     | [Mateus Fidelis](https://github.com/MatsFidelis) | [Maria Alice](https://github.com/Maliz30) |
