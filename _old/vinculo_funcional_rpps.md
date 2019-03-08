# Layout de exportação dos dados de vínculo funcional RPPS para o GestPrev Next

### Tabela de atributos (33 atributos)

    | Atributo                                | Obrigatório | Tipo      | Descrição                                                                                        | Tamanho máximo |
    | :-------------------------------------- | :---------- | :-------- | :----------------------------------------------------------------------------------------------- | -------------: |
    | data_exercicio_cargo                    | Sim         | Data      | Data de exercício no cargo, preencher no formato DD/MM/AAAA                                      | 10             |
    | data_ingresso_carreira                  | Sim         | Data      | Data de ingresso na carreira, preencher no formato DD/MM/AAAA                                    | 10             |
    | data_ingresso_orgao                     | Sim         | Data      | Data de ingresso no órgão, preencher no formato DD/MM/AAAA                                       | 10             |
    | situacao_funcional                      | Sim         | Numérico  | Situação funcional do servidor, de acordo com a Tabela 37                                        | 2              |
    | matricula                               | Sim         | Caracter  | Matrícula do servidor                                                                            | 20             |
    | regime_previdenciario                   | Sim         | Numérico  | Tipo do regime previdenciário do vínculo. [2: RPPS, 3: RPPS em extinção]                         | 1              |
    | tipo_servidor                           | Sim         | Numérico  | Tipo do servidor vinculado. [1: Civil, 2: Militar]                                               | 1              |
    | tipo_vinculo                            | Sim\*\*     | Numérico  | Tipo do vínculo do servidor com o órgão do vínculo funcional, de acordo com a Tabela 38          | 2              |
    | orgao_vinculado_nome                    | Sim         | Caracter  | Nome do órgão do vínculo funcional                                                               | 100            |
    | orgao_vinculado_poder                   | Sim         | Numérico  | Poder do órgão do vínculo funcional, de acordo com a Tabela 19                                   | 1              |
    | servidor_vinculado_nome                 | Sim         | Caracter  | Nome completo do servidor vinculado                                                              | 80             |
    | servidor_vinculado_nome_mae             | Não         | Caracter  | Nome completo da mãe do servidor vinculado                                                       | 80             |
    | servidor_vinculado_data_nascimento      | Não         | Data      | Data de nascimento do servidor vinculado, preencher no formato DD/MM/AAAA                        | 10             |
    | servidor_vinculado_cpf                  | Não         | Caracter  | CPF, preencher somente com números do servidor vinculado                                         | 11             |
    | servidor_vinculado_pasep_pis_nit        | Não         | Caracter  | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                     | 11             |
    | cargo_vinculado_nome                    | Sim         | Caracter  | Nome do cargo vinculado ao vínculo funcional                                                     | 60             |
    | cargo_vinculado_nome_carreira           | Sim         | Caracter  | Nome da carreira na qual o cargo está vinculado                                                  | 60             |
    | mov_func_abono_permanencia              | Não         | Numérico  | Recebe abono de permanência? [0: Não, 1: Sim]                                                    | 1              |
    | mov_func_abono_permanencia_data_inicio  | Não         | Data      | Data de início do abono permanência, preencher no formato DD/MM/AAAA                             | 10             |
    | mov_func_data_saida_cargo               | Não\*       | Data      | Data de saída do servidor do cargo, preencher no formato DD/MM/AAAA                              | 10             |
    | mov_func_data_inicio_rgps               | Não         | Data      | Data de início do período RGPS neste vínculo, preencher no formato DD/MM/AAAA                    | 10             |
    | mov_func_data_fim_rgps                  | Não         | Data      | Data de fim do período RGPS neste vínculo, preencher no formato DD/MM/AAAA                       | 10             |
    | mov_func_data_publicacao_cessao         | Não         | Data      | Data de publicação da portaria de cessação do servidor no cargo, preencher no formato DD/MM/AAAA | 10             |
    | mov_func_ato_nomeacao                   | Não         | Caracter  | Descrição do ato de nomeação                                                                     | 30             |
    | mov_func_classe_cargo                   | Não         | Caracter  | Código da classe do cargo, de acordo com a Tabela 39                                             | 2              |
    | mov_func_duracao_jornada                | Não         | Caracter  | Descrição da duração da jornada de trabalho                                                      | 15             |
    | mov_func_local_trabalho                 | Não         | Caracter  | Descrição do local de trabalho                                                                   | 60             |
    | mov_func_padrao_cargo                   | Não         | Caracter  | Código do padrão do cargo, de acordo com Tabela 40                                               | 2              |
    | mov_func_portaria_cessao                | Não         | Caracter  | Descrição da portaria de cessação do servidor no cargo                                           | 30             |
    | mov_func_periodo_rgps                   | Não         | Numérico  | Há período RGPS no vínculo? [0: Não, 1: Sim]                                                     | 1              |
    | mov_func_situacao_funcional             | Sim\*       | Numérico  | Situação funcional do servidor, de acordo com a Tabela 37                                        | 2              |
    | mov_func_data_movimentacao              | Sim         | Data      | Data em que ocorreu a movimentação funcional, preencher no formato DD/MM/AAAA                    | 10             |
    | mov_func_tipo_magisterio                | Sim         | Numérico  | Tipo de magistério exclusivo em sala de aula, de acordo com a Tabela 41                          | 1              |

\* Caso o servidor se encontre em situação funcional de acordo com os códigos 2, 9, 11 ou 12, o campo mov_func_data_saida_cargo deverá ser informado.

\*\* Observar a relação existente entre tipo de vínculo e tipo de regime

---

### Atributo(s) da(s) chave(s) de identificação para importação de dados

* **chave vínculo funcional RPPS**
    * regime_previdenciario, tipo_vinculo, tipo_servidor, data_exercicio_cargo, uma chave do servidor e chave do órgão

* **chave movimentação vínculo funcional RPPS**
    * mov_func_situacao_funcional, mov_func_data_movimentacao e chave vínculo funcional RPPS

* **chaves servidor (ordem de precedência)**
    1. servidor_vinculado_nome, servidor_vinculado_nome_mae, servidor_vinculado_data_nascimento
    2. servidor_vinculado_cpf
    3. servidor_vinculado_pasep_pis_nit

* **chave cargo**
    * cargo_vinculado_nome, cargo_vinculado_nome_carreira, orgao_vinculado_nome, orgao_vinculado_poder

* **chave carreira**
    * cargo_vinculado_nome_carreira, orgao_vinculado_nome, orgao_vinculado_poder

* **chave órgão**
    * orgao_vinculado_nome, orgao_vinculado_poder
