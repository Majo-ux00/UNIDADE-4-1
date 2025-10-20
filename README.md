# NORMALIZAÇÃO DE DADOS E DEPENDENCIA FUNCIONAL

Normalização de Dados e Dependência Funcional
Autor(es):
ARTHUR MARQUES GALDINO
RICARDO GOMES PEREIRA
GIOVANNA APARECIDA DOS SANTOS
MARIA JOSE TICONA RAMOS

Instituição:
ANHANGUERA - FACULDADE ANHANGUERA
Categoria do Trabalho:
Acadêmico

A normalização de dados é uma técnica formal e estruturada utilizada no projeto de bancos de dados relacionais para avaliar e corrigir as estruturas de tabelas, com o objetivo primário de minimizar a redundância de dados e, consequentemente, reduzir as chances de anomalias e inconsistências.
Objetivos Fundamentais
O propósito da normalização é garantir a qualidade e a integridade da base de dados. Ao organizar os dados de forma lógica, ela proporciona os seguintes benefícios:
Diminuição da repetição de dados, tornando o banco mais compacto e eficiente em armazenamento.
Aumento do desempenho (rendimento) do Sistema Gerenciador de Banco de Dados (SGBD) em operações de consulta e manipulação.
Facilidade na criação de consultas e no manutenção da estrutura.
Uma tabela é considerada normalizada quando trata de um único assunto e todos os seus campos não-chave são dependentes exclusivamente da chave primária daquela tabela.
Dependência Funcional (DF)
O conceito que fundamenta as formas normais (1FN, 2FN, 3FN, etc.) é a Dependência Funcional (DF).
A DF é uma restrição que define uma relação de determinação entre atributos dentro de uma tabela. A notação $X \rightarrow Y$ significa que Y é funcionalmente dependente de X, ou que X determina Y. Isso ocorre se, para cada valor específico de X, existe um e apenas um valor associado de Y.
As dependências funcionais problemáticas, que a normalização busca eliminar, são:
Dependência Parcial: Ocorre quando um atributo não-chave depende de apenas uma parte da chave primária (aplicável em chaves primárias compostas). Sua eliminação leva à Segunda Forma Normal (2FN).
Dependência Transitiva (ou Indireta): Ocorre quando um atributo não-chave (Z) depende de outro atributo não-chave (Y), que, por sua vez, depende da chave primária (X), estabelecendo o caminho $X \rightarrow Y \rightarrow Z$. Sua eliminação leva à Terceira Forma Normal (3FN).
A identificação precisa dessas dependências é o passo inicial e crucial para determinar quais tabelas exigem a decomposição e o refinamento do esquema.

REFERÊNCIAS (ABNT NBR 6023:2018)
ELMASRI, Ramez; NAVATHE, Shamkant B. Sistemas de Banco de Dados. 7. ed. São Paulo: Pearson Education do Brasil, 2018.
HEUSER, Carlos Alberto. Projeto de Banco de Dados. 6. ed. Porto Alegre: Bookman, 2009.
KORTH, Henry F.; SILBERSCHATZ, Abraham; SUDARSHAN, S. Sistema de Banco de Dados. 6. ed. Rio de Janeiro: LTC, 2011.
