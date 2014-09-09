# Layout de exportação dos dados de cargo para o GestPrev Next

### Tabela de atributos

 | Atributo                       | Obrigatório | Tipo     | Descrição                                                                | Tamanho máximo | Decimais |
 | :----------------------------- | :---------- | :------- | :----------------------------------------------------------------------- | -------------: | -------: |
 | nome                           | Sim         | Caracter | Nome do cargo                                                            | 60             | -        |
 | codigo_origem                  | Não         | Caracter | Código de origem da carreira                                             | 6              | -        |
 | data_criacao                   | Não         | Data     | Data da criação da carreira, preencher no formato DD/MM/AAAA             | 10             | -        |
 | data_extincao                  | Não         | Data     | Data da extinção da carreira, preencher no formato DD/MM/AAAA            | 10             | -        |
 | cargo_acumulacao               | Sim         | Numérico | Cargo com acumulação, de acordo com a Tabela 32                          | 1              | -        |
 | contagem_especial              | Sim         | Numérico | Cargo com contagem de tempo especial, de acordo com a Tabela 02          | 1              | -        |
 | tecnico_cientifico             | Sim         | Numérico | Cargo técnico científico. [0: Não, 1: Sim]                               | 1              | -        |
 | remuneracao_inicial            | Não         | Numérico | Valor da remuneração inicial do cargo                                    | 8              | 2        |
 | remuneracao_final              | Não         | Numérico | Valor da remuneração final do cargo                                      | 8              | 2        |
 | aposentadoria_especial         | Sim         | Numérico | Cargo tem aposentadoria especial. [0: Não, 1: Sim]                       | 1              | -        |
 | dedicacao_exclusiva            | Sim         | Numérico | Cargo com dedicação exclusiva. [0: Não, 1: Sim]                          | 1              | -        |
 | carreira_nome_carreira         | Sim         | Caracter | Nome da carreira na qual o cargo está vinculado                          | 60             | -        |
 | orgao_nome_orgao               | Sim         | Caracter | Nome do órgão vinculado à carreira do cargo                              | 100            | -        |
 | orgao_poder                    | Sim         | Numérico | Poder do órgão vinculado à carreira do cargo, de acordo com a Tabela 19  | 1              | -        |
 | ato_legal_tipo_ato             | Sim\*       | Numérico | Tipo do ato legal, de acordo com a Tabela 23                             | 2              | -        |
 | ato_legal_numero               | Sim\*       | Caracter | Número do ato legal, preencher somente com números                       | 12             | -        |
 | ato_legal_ano                  | Sim\*       | Numérico | Ano do ato legal                                                         | 4              | -        |
 | ato_legal_data_publicacao      | Sim\*       | Data     | Data de publicação do ato legal, preencher no formato DD/MM/AAAA         | 10             | -        |
 | ato_legal_data_inicio_vigencia | Sim\*       | Data     | Data de início de vigência do ato legal, preencher no formato DD/MM/AAAA | 10             | -        |
 | ato_legal_data_revogacao       | Não         | Data     | Data de revogação do ato legal, preencher no formato DD/MM/AAAA          | 10             | -        |
 | ato_legal_resumo_ementa        | Não         | Caracter | Resumo da ementa do ato legal                                            | 100            | -        |
 | ato_legal_ementa               | Não         | Caracter | Ementa do ato legal                                                      | 1000           | -        |

\* Este campo é obrigatório apenas se o Ato Legal estiver presente.

---

### Atributo(s) da(s) chave(s) de identificação para importação de dados

* **chave cargo**
    * nome, carreira_nome_carreira, orgao_nome_orgao, orgao_poder

* **chave carreira**
    * carreira_nome_carreira, orgao_nome_orgao, orgao_poder

* **chave orgão**
    * orgao_nome_orgao, orgao_poder

* **chave ato legal**
    * ato_legal_tipo_ato, ato_legal_numero, ato_legal_ano
