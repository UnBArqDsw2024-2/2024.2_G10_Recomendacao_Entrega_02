# Modelo Físico

## Introdução

O Modelo Físico de Dados é a representação mais detalhada de como os dados serão armazenados no banco de dados. Ele descreve a estrutura física real, incluindo aspectos técnicos e específicos de um sistema de gerenciamento de banco de dados (SGBD) escolhido. Essa etapa foca em transformar o Modelo Lógico de Dados em um design implementável, levando em conta restrições, performance e recursos do SGBD.

## Metodologia

Para a criação do nosso Modelo Físico de Dados, a equipe tomou a decisão de utilizar o SGBD MySQL, considerando suas funcionalidades robustas, ampla documentação e facilidade de integração com as tecnologias do nosso projeto. Esse modelo foi desenvolvido com base em três artefatos fundamentais: [Diagrama de Classes](https://unbarqdsw2024-2.github.io/2024.2_G10_Recomendacao_Entrega_02/#/modelagem-estatica/diagrama-de-classes), [Modelo Conceitual](https://unbarqdsw2024-2.github.io/2024.2_G10_Recomendacao_Entrega_02/#/modelagem-dados/modelo-conceitual) e [Modelo Lógico](https://unbarqdsw2024-2.github.io/2024.2_G10_Recomendacao_Entrega_02/#/modelagem-dados/modelo-logico).

## Modelo Físico de Dados

Abaixo é possível ver o script gerado.

```sql

-- -------- < Chefindica - Modelo Físico > --------
--
--                    SCRIPT DE CRIACAO (DDL)
--
-- Data Criacao ...........: 16/11/2024
-- Autor(es) ..............: Izabella Alves, Lucas Queiroz, Larissa Vieira, Pedro Sampaio
-- Banco de Dados .........: MySQL 8.0
-- Base de Dados (nome) ...: chefindica
--
-- PROJETO => 01 Base de Dados
--         => 05 Tabelas
--        
-- Ultimas Alteracoes
-- ---------------------------------------------------------
-- BASE DE DADOS

CREATE DATABASE IF NOT EXISTS chefindica;
USE chefindica;

-- TABELAS

CREATE TABLE Restaurante (
    id INTEGER NOT NULL AUTO_INCREMENT,
    endereco VARCHAR (100) NOT NULL,
    mediaAvaliacoes FLOAT NOT NULL,
    nome VARCHAR (100) NOT NULL,
    foto BLOB,
    CONSTRAINT Restaurante_PK PRIMARY KEY (id),
    CONSTRAINT Restaurante_UK UNIQUE (id)
)ENGINE=InnoDB;

CREATE TABLE Usuario (
    id INTEGER NOT NULL,
    nome VARCHAR (80) NOT NULL,
    senha VARCHAR (50) NOT NULL,
    email VARCHAR (100) NOT NULL,
    foto BLOB,
    CONSTRAINT Usuario_PK PRIMARY KEY (id),
    CONSTRAINT Usuario_UK UNIQUE (id, email)
)ENGINE=InnoDB;

CREATE TABLE Categoria (
    id INTEGER NOT NULL,
    nome VARCHAR (30) NOT NULL,
    CONSTRAINT Categoria_PK PRIMARY KEY (id),
    CONSTRAINT Categoria_UK UNIQUE (id, nome)
)ENGINE=InnoDB;

CREATE TABLE pertence (
    categoriaId INTEGER NOT NULL,
    restauranteId INTEGER NOT NULL,
    CONSTRAINT pertence_PK PRIMARY KEY (categoriaId, restauranteId),
    CONSTRAINT pertence_UK UNIQUE (categoriaId, restauranteId),
    CONSTRAINT pertence_Categoria_FK FOREIGN KEY (categoriaId) REFERENCES Categoria (id)
		ON DELETE RESTRICT
        ON UPDATE RESTRICT,
    CONSTRAINT pertence_Restaurante_FK FOREIGN KEY (restauranteId) REFERENCES Restaurante (id)
		ON DELETE RESTRICT
        ON UPDATE RESTRICT
)ENGINE=InnoDB;

CREATE TABLE avalia (
    usuarioId INTEGER NOT NULL,
    restauranteId INTEGER NOT NULL,
    comentario VARCHAR (300),
    nota INTEGER NOT NULL,
    dataAvaliacao DATE NOT NULL,
    CONSTRAINT avalia_PK PRIMARY KEY (usuarioId, restauranteId),
    CONSTRAINT avalia_UK UNIQUE (usuarioId, restauranteId),
    CONSTRAINT avalia_Usuario_FK FOREIGN KEY (usuarioId) REFERENCES Usuario (id)
		ON DELETE RESTRICT
        ON UPDATE RESTRICT,
    CONSTRAINT avalia_Restaurante_FK FOREIGN KEY (restauranteId) REFERENCES Restaurante (id)
		ON DELETE RESTRICT
        ON UPDATE RESTRICT
)ENGINE=InnoDB;

```

<center>
<font size="3"><p style="text-align: center"><b>Fonte:</b> <a href="https://github.com/izabellaalves">Izabella Alves</a>, <a href="https://github.com/PedroSampaioDias">Pedro Sampaio</a>, <a href="https://github.com/lucasqueiroz23">Lucas Queiroz</a> e <a href="https://github.com/VieiraLaris">Larissa Vieira</a>, 2024.</p></font>
</center>

## Bibliografia
>
> SILBERSCHATZ, Abraham; KORTH, Henry F.; SUDARSHAN, S. Sistemas de Banco de Dados. Pearson, 2011.
>

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| :----: | ---- | --------- | ----- | ------- |
| `1.0`  |16/11/2024| Adiciona script do modelo físico | [Izabella Alves](https://github.com/izabellaalves) |[Larissa Vieira](https://github.com/VieiraLaris)  |