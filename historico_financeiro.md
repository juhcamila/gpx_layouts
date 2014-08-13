# Layout de exportação dos dados de histórico financeiro para o GestPrev Next

### Tabela de atributos

    | Atributo                                     | Obrigatório | Tipo      | Descrição                                                                                        | Tamanho máximo | Decimais |
    | :--------------------------------------      | :---------- | :-------- | :----------------------------------------------------------------------------------------------- | -------------: | -------: |
    | vinc_func_data_exercicio_cargo               | Sim         | Data      | Data de exercício no cargo, preencher no formato DD/MM/AAAA                                      | 10             | -        |
    | vinc_func_data_ingresso_carreira             | Sim         | Data      | Data de ingresso na carreira, preencher no formato DD/MM/AAAA                                    | 10             | -        |
    | vinc_func_data_ingresso_orgao                | Sim         | Data      | Data de ingresso no órgão, preencher no formato DD/MM/AAAA                                       | 10             | -        |
    | vinc_func_situacao_funcional                 | Sim         | Numérico  | Situação funcional do servidor, de acordo com a Tabela 37                                        | 2              | -        |
    | vinc_func_matricula                          | Sim         | Caracter  | Matrícula do servidor                                                                            | 20             | -        |
    | vinc_func_regime_previdenciario              | Sim\*\*     | Numérico  | Tipo do regime previdenciário do vínculo. [2: RPPS, 3: RPPS em extinção]                         | 1              | -        |
    | vinc_func_tipo_servidor                      | Sim         | Numérico  | Tipo do servidor vinculado. [1: Civil, 2: Militar]                                               | 1              | -        |
    | vinc_func_tipo_vinculo                       | Sim\*\*     | Numérico  | Tipo do vínculo do servidor com o órgão do vínculo funcional, de acordo com a Tabela 38          | 2              | -        |
    | vinc_func_orgao_vinculado_nome               | Sim         | Caracter  | Nome do órgão do vínculo funcional                                                               | 100            | -        |
    | vinc_func_orgao_vinculado_poder              | Sim         | Numérico  | Poder do órgão do vínculo funcional, de acordo com a Tabela 19                                   | 1              | -        |
    | vinc_func_servidor_vinculado_nome            | Sim         | Caracter  | Nome completo do servidor vinculado                                                              | 80             | -        |
    | vinc_func_servidor_vinculado_nome_mae        | Não         | Caracter  | Nome completo da mãe do servidor vinculado                                                       | 80             | -        |
    | vinc_func_servidor_vinculado_data_nascimento | Não         | Data      | Data de nascimento do servidor vinculado, preencher no formato DD/MM/AAAA                        | 10             | -        |
    | vinc_func_servidor_vinculado_cpf             | Não         | Caracter  | CPF, preencher somente com números do servidor vinculado                                         | 11             | -        |
    | vinc_func_servidor_vinculado_pasep_pis_nit   | Não         | Caracter  | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                     | 11             | -        |
    | vinc_func_cargo_vinculado_nome               | Sim         | Caracter  | Nome do cargo vinculado ao vínculo funcional                                                     | 60             | -        |
    | vinc_func_cargo_vinculado_nome_carreira      | Sim         | Caracter  | Nome da carreira na qual o cargo está vinculado                                                  | 60             | -        |
    | hist_financ_ano_contribuicao                 | Sim         | Numérico  | Ano de contribuição do histórico financeiro                                                      | 4              | -        |
    | hist_financ_mes_contribuicao                 | Sim         | Numérico  | Mes de contribuição do histórico financeiro                                                      | 2              | -        |
    | hist_financ_base_calculo_patronal            | Não         | Numérico  | Base do cálculo de contribuição patronal do histórico financeiro                                 | 8              | 2        |
    | hist_financ_base_calculo_segurado            | Não         | Numérico  | Base do cálculo de contribuição para o segurando do histórico financeiro                         | 8              | 2        |
    | hist_financ_compoe_media_beneficio           | Sim         | Numérico  | Ficha financeira compõe média para concessão de benefício. [0: Não, 1: Sim]                      | 1              | -        |
    | hist_financ_valor_contribuicao_patronal      | Não         | Numérico  | Valor para contribuição patronal do histórico financeiro                                         | 8              | 2        |
    | hist_financ_valor_contribuicao_segurando     | Não         | Numérico  | Valor para contribuição do segurado do histórico financeiro                                      | 8              | 2        |
    | hist_financ_decimo_terceiro_salario          | Sim         | Numérico  | Ficha financeira corresponde a de 13 salário? [0: Não, 1: Sim]                                   | 1              | -        |
    | hist_financ_valor_contribuicao_devolucao     | Não         | Numérico  | Valor de devolução da contribuição do histórico financeiro                                       | 8              | 2        |
    | hist_financ_valor_contribuicao_diferenca     | Não         | Numérico  | Valor de diferença da contribuição do histórico financeiro                                       | 8              | 2        |
    | hist_financ_folha_pagamento                  | Sim         | Numérico  | Número da folha de pagamento da ficha financeira                                                 | 15             | -        |
    | hist_financ_valor_remuneracao_bruta          | Sim         | Numérico  | Valor da remuneração bruta do histórico financeiro                                               | 8              | 2        |
    | hist_financ_valor_remuneracao_cargo          | Sim         | Numérico  | Valor da remuneração do cargo do histórico financeiro                                            | 8              | 2        |
    | hist_financ_valor_remuneracao_contribuicao   | Sim\*       | Numérico  | Valor da remuneração de contribuição do histórico financeiro                                     | 8              | 2        |

\* Remuneração sobre a qual incindirá alíquota de contribuição

\*\* Observar a relação existente entre tipo de vínculo e tipo de regime
