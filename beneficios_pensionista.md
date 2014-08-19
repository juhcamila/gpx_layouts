# Layout de exportação dos dados de benefícios do pensionista para o GestPrev Next

### Tabela de atributos

 | Atributo                                | Obrigatório | Tipo      | Descrição                                                                                        | Tamanho máximo | Decimais |
 | :-------------------------------------- | :---------- | :-------- | :----------------------------------------------------------------------------------------------- | -------------: | -------: |
 | data_inicio                             | Não         | Data      | Data de início do recebimento do benefício, preencher no formato DD/MM/AAAA                      | 10             | -        |
 | tipo_beneficio                          | Sim         | Numérico  | Código do tipo do benefício, conforme Tabela 24                                                  | 2              | -        |
 | data_fim                                | Não         | Data      | Data de fim do recebimento do benefício, preencher no formato DD/MM/AAAAA                        | 10             | -        |
 | valor_atual                             | Sim         | Numérico  | Valor atual do benefício recebido pelo pensionista                                               | 8              | 2        |
 | valor_inicial                           | Não         | Numérico  | Valor inicial do benefício recebido pelo pensionista                                             | 8              | 2        |
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
 | classe_cargo                            | Não         | Caracter  | Código da classe do cargo, de acordo com a Tabela 39                                             | 2              | 0        |
 | padrao_cargo                            | Não         | Caracter  | Código do padrão do cargo, de acordo com Tabela 40                                               | 2              | 0        |
 | pensao_motivo_inicio                    | Não         | Numérico  | Código do motivo de início do benefício de pensão, conforme Tabela 14                            | 2              | -        |
 | pensao_motivo_fim                       | Não         | Numérico  | Código do motivo de fim do benefício de pensão, conforme Tabela 11                               | 2              | -        |
 | pensao_justificativa_motivo_inicio      | Não\*       | Caracter  | Justificativa do motivo de início de pensão                                                      | 50             | -        |
 | pensao_justificativa_motivo_fim         | Não\*\*     | Caracter  | Justificativa do motivo de fim de pensão                                                         | 50             | -        |
 | cargo_nome                              | Sim         | Caracter  | Nome do cargo em que o servidor se aposentou                                                     | 60             | -        |
 | carreira_nome                           | Sim         | Caracter  | Nome da carreira na qual o cargo está vinculado                                                  | 60             | -        |
 | orgao_nome                              | Sim         | Caracter  | Nome do órgão vinculado à carreira do cargo                                                      | 100            | -        |
 | orgao_poder                             | Sim         | Numérico  | Poder do órgão vinculado à carreira do cargo, de acordo com a Tabela 19                          | 1              | -        |
 | instituidor_vinculado_nome              | Sim         | Caracter  | Nome completo do instituidor vinculado                                                           | 80             | -        |
 | instituidor_vinculado_nome_mae          | Não         | Caracter  | Nome completo da mãe do instituidor vinculado                                                    | 80             | -        |
 | instituidor_vinculado_data_nascimento   | Não         | Data      | Data de nascimento do instituidor vinculado , preencher no formato DD/MM/AAAA                    | 10             | -        |
 | instituidor_vinculado_cpf               | Não         | Caracter  | CPF, preencher somente com números do instituidor vinculado                                      | 11             | -        |
 | instituidor_vinculado_pasep_pis_nit     | Não         | Caracter  | Número de PIS/PASEP/NIT do instituidor vinculado, preencher somente com números                  | 11             | -        |
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
