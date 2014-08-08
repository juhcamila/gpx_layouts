# Layout de exportação dos dados de tempo de contribuição em outro RGPS para o GestPrev Next

### Tabela de atributos

 | Atributo                           | Obrigatório | Tipo      | Descrição                                                                                    | Tamanho máximo |
 | :--------------------------------- | :---------- | :-------- | :------------------------------------------------------------------------------------------- | -------------: |
 | certidao_numero                    | Não\* \*\*  | Caractere | Número do protocolo da certidão de tempo de contribuição RGPS, preencher somente com números | 19             |
 | certidao_data_emissao              | Sim         | Data      | Data de emissão da certidao de tempo de contribuição RGPS, preencher no formato DD/MM/AAAA   | 10             |
 | pasep_pis_nit                      | Não\*\*     | Caractere | Número de PIS/PASEP/NIT do servidor, preencher somente com números                           | 11             |
 | empregador_nome                    | Não         | Caractere | Nome do empregador do tempo de contribuição RGPS                                             | 60             |
 | empregador_cnpj                    | Não         | Caractere | Número do CNPJ do empregador, preencher apenas com números                                   | 14             |
 | vinculo_data_inicial               | Sim         | Data      | Data inicial do vínculo, preencher no formato DD/MM/AAAA                                     | 10             |
 | vinculo_data_final                 | Sim         | Data      | Data final do vínculo, preencher no formato DD/MM/AAAA                                       | 10             |
 | certidao_tempo_liquido_ano_mes_dia | Sim         | Caractere | Preencher no formato AA/MM/DIA, verificar detalhes\*\*                                       | 8              |
 | certidao_numero_dias               | Sim         | Numérico  | Tempo total em dias da certidão                                                              | 5              |
 | cargo_nome                         | Sim         | Caractere | Cargo do servidor no RGPS                                                                    | 60             |
 | cargo_acumulavel                   | Não         | Numérico  | Cargo do servidor é acumulável? [0: Não, 1: Sim]                                             | 1              |
 | cargo_magisterio_exclusivo         | Não         | Numérico  | Cargo do servidor é magistério exclusivo? [0: Não, 1: Sim]                                   | 1              |
 | servico_publico                    | Não         | Numérico  | Tempo de contribuição RGPS é de serviço público? [0: Não, 1: Sim]                            | 1              |
 | servidor_vinculado_nome            | Sim         | Caracter  | Nome completo do servidor vinculado                                                          | 80             |
 | servidor_vinculado_nome_mae        | Não         | Caracter  | Nome completo da mãe do servidor vinculado                                                   | 80             |
 | servidor_vinculado_data_nascimento | Não         | Data      | Data de nascimento do servidor vinculado, preencher no formato DD/MM/AAAA                    | 10             |
 | servidor_vinculado_cpf             | Não         | Caracter  | CPF, preencher somente com números do servidor vinculado                                     | 11             |
 | servidor_vinculado_pasep_pis_nit   | Não         | Caracter  | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                 | 11             |

\* Campo obrigatório para certidões emitidas após 01/09/1994

\*\* Caso o servidor possua mais de um vínculo empregatício na certidão, os atributos certidao_numero, certidao_data_emissao e pasep_pis_nit serão necessários para compor a chave composta para cadastramento dos vincínculos empregatícios
