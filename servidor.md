# Layout de exportação dos dados de servidores para o GestPrev Next

### Tabela de atributos

 | Atributo                                            | Obrigatório | Tipo     | Descrição                                                                                                    | Tamanho máximo |
 | :-------------------------------------------------- | :---------- | :------- | :----------------------------------------------------------------------------------------------------------- | -------------: |
 | nome                                                | Sim         | Caracter | Nome completo                                                                                                | 80             |
 | nome_mae                                            | Não         | Caracter | Nome completo da mãe                                                                                         | 80             |
 | data_nascimento                                     | Não         | Data     | Data de nascimento, preencher no formato DD/MM/AAAA                                                          | 10             |
 | cpf                                                 | Não         | Caracter | CPF, preencher somente com números                                                                           | 11             |
 | nome_pai                                            | Não         | Caracter | Nome completo do pai                                                                                         | 80             |
 | rg                                                  | Não         | Caracter | RG do servidor                                                                                               | 20             |
 | rg_uf_expedicao                                     | Não         | Numérico | Código IBGE da UF de expedição do RG, de acordo com a Tabela 08                                              | 8              |
 | rg_orgao_expedidor                                  | Não         | Numérico | Código do órgão expedidor do RG, de acordo com a Tabela 16                                                   | -              |
 | rg_data_emissao                                     | Não         | Data     | Data de emissão do RG, preencher no formato DD/MM/AAAA                                                       | 10             |
 | estado_civil                                        | Não         | Numérico | Código do estado civil, de acordo com a Tabela 06                                                            | 2              |
 | email                                               | Não         | Caracter | Correio eletrônico                                                                                           | 80             |
 | email_institucional                                 | Não         | Caracter | Correio eletrônico institucional                                                                             | 80             |
 | tipo_sanguineo                                      | Não         | Numérico | Tipo sanguíneo, de acordo com a Tabela 29                                                                    | -              |
 | escolaridade_nivel                                  | Não         | Numérico | Escolaridade, de acordo com a Tabela 04                                                                      | -              |
 | escolaridade_nome_curso                             | Não         | Caracter | Nome do curso acadêmico                                                                                      | 100            |
 | escolaridade_nome_instituicao                       | Não         | Caracter | Nome da instituição do curso acadêmico                                                                       | 100            |
 | escolaridade_ano_conclusao                          | Não         | Data     | Ano de conclusão do curso acadêmico, preencher no formato DD/MM/AAAA                                         | 10             |
 | sexo                                                | Não         | Numérico | Sexo [0: Masculino, 1: Feminino]                                                                             | 1              |
 | tipo_deficiencia                                    | Não         | Numérico | Tipo de deficiência, de acordo com a Tabela 25                                                               | 1              |
 | pais_origem                                         | Não         | Numérico | Nacionalidade, código do país de origem do servidor, de acordo com a Tabela 18                               | -              |
 | municipio_naturalidade                              | Não         | Numérico | Código IBGE do município de naturalidade do servidor, de acordo com a Tabela 07                              | 8              |
 | endereco_cep                                        | Não         | Caracter | CEP do endereço, preencher somente com números                                                               | 8              |
 | endereco_municipio                                  | Não         | Numérico | Código IBGE do município atual, de acordo com a Tabela 07                                                    | 8              |
 | endereco_logradouro_tipo                            | Não         | Numérico | Tipo do logradouro, de acordo com a Tabela 08                                                                | 2              |
 | endereco_tipo_imovel                                | Não         | Numérico | Tipo de imóvel, de acordo com a Tabela 27                                                                    | 2              |
 | endereco_bairro                                     | Não         | Caracter | Bairro                                                                                                       | 30             |
 | endereco_logradouro                                 | Não         | Caracter | Logradouro                                                                                                   | 40             |
 | endereco_logradouro_complemento                     | Não         | Caracter | Complemento do logradouro                                                                                    | 30             |
 | endereco_logradouro_numero                          | Não         | Caracter | Número do logradouro, preencher somente com números                                                          | 5              |
 | telefone_ddd                                        | Não         | Caracter | DDD do telefone                                                                                              | 2              |
 | telefone                                            | Não         | Caracter | Número do telefone, preencher somente com números                                                            | 9              |
 | celular_ddd                                         | Não         | Caracter | DDD do celular                                                                                               | 2              |
 | celular                                             | Não         | Caracter | Número do celular, preencher somente com números                                                             | 9              |
 | pasep_pis_nit                                       | Não         | Caracter | Número de PIS/PASEP/NIT, preencher somente com números                                                       | 11             |
 | cor_raca                                            | Não         | Numérico | Cor/raça, de acordo com a Tabela 03                                                                          | -              |
 | data_ingresso_servico_publico                       | Não         | Data     | Data de ingresso no serviço público, preencher no formato DD/MM/AAAA                                         | 10             |
 | cnh                                                 | Não         | Caracter | Número da CNH, preencher somente com números                                                                 | -              |
 | cnh_data_emissao                                    | Não         | Data     | Data de emissão da CNH, preencher no formato DD/MM/AAAA                                                      | 10             |
 | cnh_data_validade                                   | Não         | Data     | Data de validade da CNH, preencher no formato DD/MM/AAAA                                                     | 10             |
 | cnh_categorias                                      | Não         | Caracter | Categorias da CNH, de acordo com a Tabela 33                                                                 | 2              |
 | ctps                                                | Não         | Numérico | Número da CTPS, preencher somente com números                                                                | 8              |
 | ctps_serie                                          | Não         | Caracter | Série da CTPS                                                                                                | 10             |
 | ctps_data_emissao                                   | Não         | Data     | Data de emissão da CTPS, preencher no formato DD/MM/AAAA                                                     | 10             |
 | ctps_uf_expedicao                                   | Não         | Numérico | Código IBGE da UF de expedição da CTPS, de acordo com a Tabela 08                                            | 8              |
 | titulo_eleitor_numero                               | Não         | Caracter | Número do título de eleitor, preencher somente com números                                                   | 14             |
 | titulo_eleitor_zona                                 | Não         | Numérico | Zona do título de eleitor                                                                                    | -              |
 | titulo_eleitor_secao_eleitoral                      | Não         | Numérico | Seção do título de eleitor                                                                                   | -              |
 | titulo_eleitor_uf_expedicao                         | Não         | Numérico | Código IBGE da UF de emissão do título de eleitor, de acordo com a Tabela 08                                 | -              |
 | data_falecimento                                    | Não         | Data     | Data de falecimento do servidor, preencher no formato DD/MM/AAAA                                             | 10             |
 | certidao_obito_termo                                | Não         | Caracter | Número do termo da certidão de óbito, preencher somente com números                                          | 15             |
 | certidao_obito_livro                                | Não         | Caracter | Número do livro da certidão de óbito, preencher somente com números                                          | 15             |
 | certidao_obito_folha                                | Não         | Caracter | Número da folha da certidão de óbito, preencher somente com números                                          | 6              |
 | certidao_obito_data_emissao                         | Não         | Data     | Data de emissão da certidão de óbito, preencher no formato DD/MM/AAAA                                        | 10             |
 | cartorio_obito_cnpj                                 | Não         | Caracter | CNPJ do cartório de registro do óbito, preencher somente com números                                         | 8              |
 | cartorio_obito_nome                                 | Não         | Caracter | Nome do cartório de registro do óbito                                                                        | 40             |
 | cartorio_obito_cep                                  | Não         | Caracter | CEP do cartório de registro do óbito, preencher somente com números                                          | 8              |
 | cartorio_obito_municipio                            | Não         | Numérico | Código IBGE do município do cartório de registro do óbito, de acordo com a Tabela 07                         | 8              |
 | cartorio_obito_logradouro_tipo                      | Não         | Numérico | Tipo de logradouro do cartório de registro do óbito, de acordo com a Tabela 28                               | 2              |
 | cartorio_obito_bairro                               | Não         | Caracter | Bairro do cartório de registro do óbito                                                                      | 30             |
 | cartorio_obito_logradouro                           | Não         | Caracter | Logradouro do cartório de registro do óbito                                                                  | 40             |
 | cartorio_obito_logradouro_complemento               | Não         | Caracter | Complemento do logradouro do cartório de registro do óbito                                                   | 30             |
 | cartorio_obito_logradouro_numero                    | Não         | Caracter | Número do logradouro do cartório de registro do óbito, preencher somente com números                         | 5              |
 | estrangeiro_naturalizado                            | Não         | Numérico | Se o servidor é naturalizado, para nacionalidade diferente de Brasileira. [0: Não, 1: Sim]                   | 1              |
 | estrangeiro_visto_permanente                        | Não         | Numérico | Visto permanente para nacionalidade diferente de Brasileira. [0: Não, 1: Sim]                                | 1              |
 | estrangeiro_data_chegada_brasil                     | Não         | Data     | Data de chegada ao Brasil para nacionalidade diferente de Brasileira, preencher no formato DD/MM/AAAA        | 10             |
 | estrangeiro_rg                                      | Não         | Caracter | Número do RGE, para nacionalidade diferente de Brasileira                                                    | 20             |
 | estrangeiro_rg_orgao_emissor                        | Não         | Caracter | Preencher com o nome do órgão expedição/emissor do RGE, para nacionalidade diferente de Brasileira           | -              |
 | estrangeiro_rg_uf_expedicao                         | Não         | Numérico | Código IBGE da UF de expedição do RGE, de acordo com a Tabela 08, para nacionalidade diferente de Brasileira | 8              |
 | estrangeiro_rg_data_emissao                         | Não         | Data     | Data de emissão do RGE, preencher no formato DD/MM/AAAA, para nacionalidade diferente de Brasileira          | 10             |
 | conselho_classe_nome                                | Não         | Caracter | Nome do conselho de classe                                                                                   | 60             |
 | conselho_classe_numero                              | Não         | Caracter | Número do conselho de classe                                                                                 | 8              |
 | conselho_classe_uf_expedicao                        | Não         | Numérico | Código IBGE da UF de expedição do conselho de classe, de acordo com a Tabela 08                              | 8              |
 | conselho_classe_data_emissao                        | Não         | Data     | Data de emissão da carteira de conselho de classe, preencher no formato DD/MM/AAAA                           | 10             |
 | conselho_classe_data_validade                       | Não         | Data     | Data de validade da carteira de conselho de classe, preencher no formato DD/MM/AAAA                          | 10             |
 | assistencia_saude_rede_atendimento                  | Não         | Numérico | Tipo da rede de atendimento. [0: Pública, 1: Privada]                                                        | 1              |
 | assistencia_saude_plano_operadora                   | Não         | Caracter | Nome da operadora do plano de Saúde                                                                          | 100            |
 | assistencia_saude_plano_nome                        | Não         | Caracter | Nome do plano de saúde                                                                                       | 100            |
 | assistencia_saude_plano_titular                     | Não         | Numérico | Servidor titular ou dependente. [0: Titular, 1: Dependente]                                                  | 1              |
 | informatica_conhecimentos_gerais                    | Não         | Numérico | Conhecimentos gerais de informática, de acordo com a Tabela 34                                               | 1              |
 | informatica_conhecimentos_nivel                     | Não         | Numérico | Nível de conhecimento em informática, de acordo com a Tabela 35                                              | 1              |
 | representatividade_tipo                             | Sim*        | Numérico | Tipo da representatividade do servidor para com seu representante legal, de acordo com a Tabela 36           | 1              |
 | representatividade_data_inicio                      | Não\*\*     | Data     | Data de início da representatividade, preencher no formato DD/MM/AAAA                                        | 10             |
 | representatividade_data_termino_previsto            | Não\*\*\*   | Data     | Data de término previsto da representatividade, preencher no formato DD/MM/AAAA                              | 10             |
 | representante_legal_nome                            | Sim\*       | Caracter | Nome do representante legal                                                                                  | 80             |
 | representante_legal_cpf                             | Sim\*       | Caracter | CPF do representante legal, preencher somente com números                                                    | 11             |
 | representante_legal_rg                              | Sim\*       | Caracter | RG do representante legal                                                                                    | 20             |
 | representante_legal_rg_orgao_expedidor              | Não         | Numérico | Código do órgão expedidor do RG, de acordo com a Tabela 16                                                   | -              |
 | representante_legal_rg_uf_expedicao                 | Não         | Caracter | Código IBGE da UF de expedição do RG do representante legal, de acordo com a Tabela 08                       | 8              |
 | representante_legal_rg_data_emissao                 | Não         | Data     | Data de emissão do RG do representante legal, preencher no formato DD/MM/AAAA                                | 10             |
 | representante_legal_data_nascimento                 | Sim\*       | Data     | Data de nascimento do representante legal, preencher no formato DD/MM/AAAA                                   | 10             |
 | representante_legal_sexo                            | Sim\*       | Numérico | Sexo do representante legal. [0: Masculino, 1: Feminino]                                                     | 1              |
 | representante_legal_endereco_cep                    | Não         | Caracter | CEP do endereço do representante legal, preencher somente com números                                        | 8              |
 | representante_legal_endereco_municipio              | Não         | Numérico | Código IBGE do município do representante legal, de acordo com a Tabela 07                                   | 8              |
 | representante_legal_endereco_logradouro_tipo        | Não         | Numérico | Tipo do logradouro do representante legal, de acordo com a Tabela 08                                         | 2              |
 | representante_legal_endereco_tipo_imovel            | Não         | Numérico | Tipo de imóvel do representante legal, de acordo com a Tabela 27                                             | 2              |
 | representante_legal_endereco_bairro                 | Não         | Caracter | Bairro do representante legal                                                                                | 30             |
 | representante_legal_endereco_logradouro             | Não         | Caracter | Logradouro do representante legal                                                                            | 40             |
 | representante_legal_endereco_logradouro_complemento | Não         | Caracter | Complemento do logradouro do representante legal                                                             | 30             |
 | representante_legal_endereco_logradouro_numero      | Não         | Caracter | Número do logradouro do representante legal, preencher somente com números                                   | 5              |
 | representante_legal_telefone_ddd                    | Não         | Caracter | DDD do telefone do representante legal                                                                       | 2              |
 | representante_legal_telefone                        | Não         | Caracter | Número do telefone do representante legal, preencher somente com números                                     | 9              |
 | representante_legal_celular_ddd                     | Não         | Caracter | DDD do celular do representante legal                                                                        | 2              |
 | representante_legal_celular                         | Não         | Caracter | Número do celular do representante legal, preencher somente com números                                      | 9              |
 | representante_legal_email                           | Não         | Caracter | Correio eletrônico                                                                                           | 80             |

\* Campos obrigatórios apenas se o representante legal e o tipo de representatividade do servidor estiverem presentes

\*\* Este campo torna-se obrigatório caso o campo representatividade_tipo contenha o valor 4 ou 5.

\*\*\* Este campo torna-se obrigatório caso o campo representatividade_tipo contenha o valor 5.
