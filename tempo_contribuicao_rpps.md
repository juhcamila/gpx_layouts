# Layout de exportação dos dados de tempo de contribuição em outro RPPS para o GestPrev Next

### Tabela de atributos

 | Atributo                                | Obrigatório | Tipo      | Descrição                                                                                      | Tamanho máximo |
 | :-------------------------------------- | :---------- | :-------- | :--------------------------------------------------------------------------------------------- | -------------: |
 | rpps_certidao_numero                    | Não\*       | Caracter  | Número do protocolo da certidão de tempo de contribuição RPPS, preencher somente com números   | 12             |
 | rpps_certidao_data_emissao              | Sim         | Data      | Data de emissão da certidao de tempo de contribuição RPPS, preencher no formato DD/MM/AAAA     | 10             |
 | rpps_cnpj                               | Sim         | Caracter  | Número do CNPJ do Ente Federativo, preencher apenas com números                                | 14             |
 | rpps_certidao_orgao_expedidor           | Não         | Caractere | Nome do órgão do RPPS que expediu a certidão de tempo de contribuição                          | 60             |
 | rpps_certidao_nome_dirigente            | Não         | Caractere | Nome do dirigente da RPPS que forneceu a certidão de tempo de contribuição                     | 50             |
 | rpps_vinculo_data_inicial               | Sim         | Data      | Data inicial do vínculo com o RPPS, preencher no formato DD/MM/AAAA                            | 10             |
 | rpps_vinculo_data_final                 | Sim         | Data      | Data final do vínculo com o RPPS, preencher no formato DD/MM/AAAA                              | 10             |
 | rpps_certidao_tempo_liquido_ano_mes_dia | Sim         | Caractere | Preencher no formato AA/MM/DIA, verificar detalhes\*\*                                         | 8              |
 | rpps_certidao_numero_dias               | Sim         | Numérico  | Tempo total em dias da certidão de tempo de contribuição RPPS                                  | 5              |
 | rpps_certidao_responsavel_homologacao   | Não         | Caractere | Nome do responsável pela homolgação da certidão de tempo de contribuição RPPS                  | 50             |
 | rpps_matricula_numero                   | Não         | Caractere | Matrícula do servidor no RPPS que expediu a certidão de tempo de contribuição                  | 8              |
 | rpps_cargo_efetivo_nome                 | Sim         | Caractere | Nome do cargo efetivo do servidor no RPPS que expediu a certidão de tempo de contribuição      | 60             |
 | rpps_certidao_data_homologacao          | Não         | Data      | Data da homologação da certidão de tempo de contribuição RPPS, preencher no formato DD/MM/AAAA | 10             |
 | rpps_cargo_acumulavel                   | Não         | Numérico  | Cargo do servidor é acumulável?. [0: Não, 1: Sim]                                              | 1              |
 | rpps_cargo_magisterio_exclusivo         | Não         | Numérico  | Cargo do servidor é magistério exclusivo?. [0: Não, 1: Sim]                                    | 1              |
 | servidor_vinculado_nome                 | Sim         | Caracter  | Nome completo do servidor vinculado                                                            | 80             |
 | servidor_vinculado_nome_mae             | Não         | Caracter  | Nome completo da mãe do servidor vinculado                                                     | 80             |
 | servidor_vinculado_data_nascimento      | Não         | Data      | Data de nascimento do servidor vinculado , preencher no formato DD/MM/AAAA                     | 10             |
 | servidor_vinculado_cpf                  | Não         | Caracter  | CPF, preencher somente com números do servidor vinculado                                       | 11             |
 | servidor_vinculado_pasep_pis_nit        | Não         | Caracter  | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                   | 11             |

\* Campo obrigatório para certidões emitidas após 16/05/2008

\*\* Formato do campo deve ser AA/MM/DD, sendo meses de 01 até 12 e dias de 01 até 30. Exemplos: 15/11/09 (15 anos, 11 meses e 9 dias)
