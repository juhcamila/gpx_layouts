# Layout de exportação dos dados de benefício do servidor para o GestPrev Next

### Tabela de atributos

 | Atributo                                | Obrigatório | Tipo      | Descrição                                                                                        | Tamanho máximo | Decimais |
 | :-------------------------------------- | :---------- | :-------- | :----------------------------------------------------------------------------------------------- | -------------: | -------: |
 | data_inicio                             | Não         | Data      | Data de início do recebimento do benefício, preencher no formato DD/MM/AAAA                      | 10             | -        |
 | tipo_beneficio                          | Sim         | Numérico  | Código do tipo do benefício, conforme Tabela 24                                                  | 2              | -        |
 | data_fim                                | Não         | Data      | Data de fim do recebimento do benefício, preencher no formato DD/MM/AAAAA                        | 10             | -        |
 | valor_atual                             | Sim         | Numérico  | Valor atual do benefício recebido pelo servidor                                                  | 8              | 2        |
 | valor_inicial                           | Não         | Numérico  | Valor inicial do benefício recebido pelo servidor                                                | 8              | 2        |
 | numero_processo                         | Não         | Numérico  | Número do processo do benefício do servidor                                                      | 20             | -        |
 | numero_beneficio                        | Não         | Numérico  | Número do benefício do servidor                                                                  | 20             | -        |
 | data_ultima_atualizacao                 | Sim         | Data      | Data da última atualização no benefício, preencher no formato DD/MM/AAAA                         | 10             | -        |
 | data_publicacao                         | Não         | Data      | Data de publicação do benefício, preencher no formato DD/MM/AAAA                                 | 10             | -        |
 | trib_conta_nome_responsavel             | Não         | Caracter  | Nome do responsável pelo registrou ou homologação no tribunal de contas                          | 100            | -        |
 | trib_conta_data_registro_homologacao    | Não         | Data      | Data do registro ou homologação no tribunal de contas, preenhcer no formato DD/MM/AAAA           | 10             | -        |
 | trib_conta_resumo_ato_legal             | Não         | Caracter  | Resumo do documento de ato legal com registro ou homologação no tribunal de contas               | 1000           | -        |
 | trib_conta_documento_ato_legal          | Não         | Caracter  | Identificação do documento de ato legal com registro ou homologação no tribunal de contas        | 60             | -        |
 | paridade                                | Não         | Numérico  | Aposentadoria concedida com paridade? [0: Não, 1: Sim]                                           | 1              | -        |
 | regime                                  | Não         | Numérico  | Regime no o servidor se aposentou. [1: RGPS, 2: RPPS, 3: RPPS em extinção]                       | 1              | -        |
 | tempo_total_dias_rgps                   | Não         | Numérico  | Tempo total em dias no RGPS considerado para a aposentadoria                                     | 5              | 0        |
 | tempo_total_dias_rpps                   | Não         | Numérico  | Tempo total em dias no RPPS considerado para a aposentadoria                                     | 5              | 0        |
 | classe_cargo                            | Não         | Caracter  | Código da classe do cargo, de acordo com a Tabela 39                                             | 2              | 0        |
 | padrao_cargo                            | Não         | Caracter  | Código do padrão do cargo, de acordo com Tabela 40                                               | 2              | 0        |
 | salario_familia_quantidade_dependentes  | Não         | Numérico  | Quantidade de dependentes do salário família                                                     | 2              | -        |
 | salario_familia_valor_total             | Não         | Numérico  | Valor do salário família total                                                                   | 8              | 2        |
 | salario_familia_valor_individual        | Não         | Numérico  | Valor do salário família individual                                                              | 8              | 2        |
 | reclusao_declaracao_numero              | Não         | Caracter  | Número da declaração da reclusão, preencher somente com números                                  | 20             | -        |
 | reclusao_declaracao_data                | Não         | Data      | Data da declaração da reclusão, preencher no formato DD/MM/AAAA                                  | 10             | -        |
 | data_encarceramento                     | Não         | Data      | Data do encarceramento, preencher no formato DD/MM/AAAA                                          | 10             | -        |
 | tipo_aposentadoria_especial             | Não         | Numérico  | Código do tipo de aposentadoria especial, conforme Tabela 22                                     | 2              | -        |
 | pensao_motivo_inicio                    | Não         | Numérico  | Código do motivo de início do benefício de pensão, conforme Tabela 14                            | 2              | -        |
 | pensao_motivo_fim                       | Não         | Numérico  | Código do motivo de fim do benefício de pensão, conforme Tabela 11                               | 2              | -        |
 | pensao_justificativa_motivo_inicio      | Não\*       | Caracter  | Justificativa do motivo de início de pensão                                                      | 50             | -        |
 | pensao_justificativa_motivo_fim         | Não \*\*    | Caracter  | Justificativa do motivo de fim de pensão                                                         | 50             | -        |
 | reclusao_motivo_inicio_auxilio          | Não         | Numérico  | Código do motivo de início do benefício de auxílio reclusão, conforme Tabela 12                  | 1              | -        |
 | reclusao_motivo_fim_auxilio             | Não         | Numérico  | Código do motivo de fim do benefício de auxílio reclusão, conforme Tabela 9                      | 1              | -        |
 | ato_legal_tipo_ato                      | Sim \*\*\*  | Numérico  | Tipo do ato legal, de acordo com a Tabela 23                                                     | 2              | -        |
 | ato_legal_numero                        | Sim \*\*\*  | Caracter  | Número do ato legal, preencher somente com números                                               | 12             | -        |
 | ato_legal_ano                           | Sim \*\*\*  | Numérico  | Ano do ato legal                                                                                 | 4              | -        |
 | ato_legal_data_publicacao               | Sim \*\*\*  | Data      | Data de publicação do ato legal, preencher no formato DD/MM/AAAA                                 | 10             | -        |
 | ato_legal_data_inicio_vigencia          | Sim \*\*\*  | Data      | Data de início de vigência do ato legal, preencher no formato DD/MM/AAAA                         | 10             | -        |
 | ato_legal_data_revogacao                | Não         | Data      | Data de revogação do ato legal, preencher no formato DD/MM/AAAA                                  | 10             | -        |
 | ato_legal_resumo_ementa                 | Não         | Caracter  | Resumo da ementa do ato legal                                                                    | 100            | -        |
 | ato_legal_ementa                        | Não         | Caracter  | Ementa do ato legal                                                                              | 1000           | -        |
 | cargo_nome                              | Sim         | Caracter  | Nome do cargo em que o servidor se aposentou                                                     | 60             | -        |
 | carreira_nome                           | Sim         | Caracter  | Nome da carreira na qual o cargo está vinculado                                                  | 60             | -        |
 | orgao_nome                              | Sim         | Caracter  | Nome do órgão vinculado à carreira do cargo                                                      | 100            | -        |
 | orgao_poder                             | Sim         | Numérico  | Poder do órgão vinculado à carreira do cargo, de acordo com a Tabela 19                          | 1              | -        |
 | servidor_vinculado_nome                 | Sim         | Caracter  | Nome completo do servidor vinculado                                                              | 80             | -        |
 | servidor_vinculado_nome_mae             | Não         | Caracter  | Nome completo da mãe do servidor vinculado                                                       | 80             | -        |
 | servidor_vinculado_data_nascimento      | Não         | Data      | Data de nascimento do servidor vinculado , preencher no formato DD/MM/AAAA                       | 10             | -        |
 | servidor_vinculado_cpf                  | Não         | Caracter  | CPF, preencher somente com números do servidor vinculado                                         | 11             | -        |
 | servidor_vinculado_pasep_pis_nit        | Não         | Caracter  | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                     | 11             | -        |
 | quota_data_inicio_pensao                | Não         | Data      | Data de início do recebimento da pensão, preencher no formato DD/MM/AAAA                         | 10             | -        |
 | quota_data_fim_pensao                   | Não         | Data      | Data final do recebimento de pensão, preencher no formato DD/MM/AAAA                             | 10             | -        |
 | quota_valor                             | Não         | Numérico  | Valor da quota em termos percentual                                                              | 3              | 2        |
 | quota_matricula                         | Não         | Caracter  | Número da matrícula do pensionista                                                               | 20             | -        |
 | pensionista_vinculado_nome              | Sim         | Caracter  | Nome completo do pensionista vinculado                                                           | 80             | -        |
 | pensionista_vinculado_nome_mae          | Não         | Caracter  | Nome completo da mãe do pensionista vinculado                                                    | 80             | -        |
 | pensionista_vinculado_data_nascimento   | Não         | Data      | Data de nascimento do pensionista vinculado , preencher no formato DD/MM/AAAA                    | 10             | -        |
 | pensionista_vinculado_cpf               | Não         | Caracter  | CPF, preencher somente com números do pensionista vinculado                                      | 11             | -        |
 | pensionista_vinculado_pasep_pis_nit     | Não         | Caracter  | Número de PIS/PASEP/NIT do pensionista vinculado, preencher somente com números                  | 11             | -        |
 | dependente_vinculado_nome               | Sim         | Caracter  | Nome completo do dependente vinculado                                                            | 80             | -        |
 | dependente_vinculado_nome_mae           | Não         | Caracter  | Nome completo da mãe do dependente vinculado                                                     | 80             | -        |
 | dependente_vinculado_data_nascimento    | Não         | Data      | Data de nascimento do dependente vinculado , preencher no formato DD/MM/AAAA                     | 10             | -        |
 | dependente_vinculado_cpf                | Não         | Caracter  | CPF, preencher somente com números do dependente vinculado                                       | 11             | -        |
 | dependente_vinculado_pasep_pis_nit      | Não         | Caracter  | Número de PIS/PASEP/NIT do dependente vinculado, preencher somente com números                   | 11             | -        |

\* Este campo torna-se obrigatório caso o atributo pensao_motivo_inicio contenha código diferente de 10 ("Óbito")

\*\* Este campo torna-se obrigatório caso o atributo pensao_motivo_fim contenha código diferente de de 51 ou 99 ("Decisão Judicial" ou "Outros")

\*\*\* Este campo é obrigatório apenas se o Ato Legal estiver presente
