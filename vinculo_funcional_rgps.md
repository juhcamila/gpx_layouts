# Layout de exportação dos dados de vínculo funcional RGPS para o GestPrev Next

### Tabela de atributos

 | Atributo                                | Obrigatório | Tipo      | Descrição                                                                                               | Tamanho máximo |
 | :-------------------------------------- | :---------- | :-------- | :-----------------------------------------------------------------------------------------------        | -------------: |
 | data_inicio_funcao                      | Sim         | Data      | Data de início na função/emprego, preencher no formato DD/MM/AAAA                                       | 10             |
 | descricao_funcao                        | Sim         | Caracter  | Nome da função ou emprego exercido pelo servidor no RGPS                                                | 25             |
 | matricula                               | Sim         | Caracter  | Matrícula do servidor                                                                                   | 20             |
 | regime_previdenciario                   | Sim         | Numérico  | Tipo do regime previdenciário do vínculo. [1: RGPS]                                                     | 1              |
 | tipo_vinculo                            | Sim\*       | Numérico  | Tipo do vínculo do servidor com o órgão do vínculo funcional, de acordo com a Tabela 38                 | 2              |
 | vereador                                | Não         | Numérico  | Servidor exerce mandato como vereador? [0: Não, 1: Sim]                                                 | 1              |
 | orgao_vinculado_nome                    | Sim         | Caracter  | Nome do órgão do vínculo funcional                                                                      | 100            |
 | orgao_vinculado_poder                   | Sim         | Numérico  | Poder do órgão do vínculo funcional, de acordo com a Tabela 19                                          | 1              |
 | servidor_vinculado_nome                 | Sim         | Caracter  | Nome completo do servidor vinculado                                                                     | 80             |
 | servidor_vinculado_nome_mae             | Não         | Caracter  | Nome completo da mãe do servidor vinculado                                                              | 80             |
 | servidor_vinculado_data_nascimento      | Não         | Data      | Data de nascimento do servidor vinculado, preencher no formato DD/MM/AAAA                               | 10             |
 | servidor_vinculado_cpf                  | Não         | Caracter  | CPF, preencher somente com números do servidor vinculado                                                | 11             |
 | servidor_vinculado_pasep_pis_nit        | Não         | Caracter  | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                            | 11             |
 | mov_func_data_fim_funcao                | Não         | Data      | Data final na função/emprego, preencher no formato DD/MM/AAAA                                           | 10             |
 | mov_func_data_movimentacao              | Sim         | Data      | Data em que ocorreu a movimentação funcional, preencher no formato DD/MM/AAAA                           | 10             |
 | mov_func_descricao_funcao               | Sim         | Caracter  | Nome da função/emprego exercido pelo servidor no RGPS                                                   | 25             |
 | mov_func_ato_legal_tipo                 | Sim         | Numérico  | Tipo do ato legal do histórico funcional do RGPS, de acordo com Tabela 23                               | 2              |
 | mov_func_ato_legal_numero               | Sim         | Numérico  | Número do ato legal do histórico funcional do RGPS                                                      | 12             |
 | mov_func_ato_legal_ano                  | Sim         | Numérico  | Ano do ato legal do histórico funcional do RGPS                                                         | 4              |
 | mov_func_ato_legal_data_publicacao      | Sim         | Data      | Data de publicação do ato legal do histórico funcional do RGPS, preencher no formato DD/MM/AAAA         | 10             |
 | mov_func_ato_legal_data_inicio_vigencia | Sim         | Data      | Data de início de vigência do ato legal do histórico funcional do RGPS, preencher no formato DD/MM/AAAA | 10             |
 | mov_func_ato_legal_data_revogacao       | Não         | Data      | Data de revogação do ato legal do histórico funcional do RGPS, preencher no formato DD/MM/AAAA          | 10             |
 | mov_func_ato_legal_resumo_ementa        | Não         | Caracter  | Resumo da ementa do ato legal do histórico funcional do RGPS                                            | 100            |
 | mov_func_ato_legal_ementa               | Não         | Caracter  | Ementa do ato legal do histórico funcional do RGPS                                                      | 1000           |

\* Observar a relação existente entre tipo de vínculo e tipo de regime
