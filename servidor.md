# Layout de exportação dos dados de servidores para o GestPrev Next

### Observações:

 - O arquivo deve estar em formato CSV **com header** e separado por “,”.
 - Tanto os headers quanto os valores devem estar entre "aspas duplas".
 - Os campos não podem conter caracteres especiais que não sejam acentos. Exemplo: “, ‘, ;.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente devem conter uma casa decimal. Exemplo: “100.0” ou “456.78”.
 - A coluna tamanho informa o limite máximo de caracteres aceitáveis na coluna. Não é necessário preencher o resto com espaço.

### Tabela de atributos

 | Atributo                              | Obrigatório | Tipo     | Descrição                                                                            | Tamanho máximo |
 | :------------------------------------ | :---------- | :------- | :----------------------------------------------------------------------------------- | -------------: |
 | nome                                  | Sim         | Caracter | Nome completo                                                                        | 80             |
 | nome_mae                              | Não         | Caracter | Nome completo da mãe                                                                 | 80             |
 | data_nascimento                       | Não         | Caracter | Data de nascimento, preencher no formato DD/MM/AAAA                                  | 10             |
 | cpf                                   | Não         | Caracter | CPF, preencher somente com números                                                   | 11             |
 | nome_pai                              | Não         | Caracter | Nome completo do pai                                                                 | 80             |
 | rg                                    | Não         | Caracter | Número do RG, preencher somente com números                                          | 20             |
 | rg_uf_expedicao                       | Não         | Numérico | Código IBGE da UF de expedição do RG, de acordo com a Tabela 08                      | 8              |
 | rg_orgao_emissor                      | Não         | Numérico | Código do órgão emissor do RG, de acordo com a Tabela 16                             | -              |
 | rg_data_expedicao                     | Não         | Caracter | Data de expedição do RG, preencher no formato DD/MM/AAAA                             | 10             |
 | estado_civil                          | Não         | Numérico | Código do estado civil, de acordo com a Tabela 06                                    | 2              |
 | email                                 | Não         | Caracter | Correio eletrônico                                                                   | 80             |
 | tipo_sanguineo                        | Não         | Numérico | Tipo sanguíneo, de acordo com a Tabela 29                                            | -              |
 | escolaridade                          | Não         | Numérico | Escolaridade, de acordo com a Tabela 04                                              | -              |
 | sexo                                  | Não         | Numérico | Sexo [0: Masculino, 1: Feminino]                                                     | 1              |
 | tipo_deficiencia                      | Não         | Numérico | Tipo de deficiência, de acordo com a Tabela 25                                       | 1              |
 | naturalizado                          | Não         | Numérico | Se o servidor é naturalizado [0: Não, 1: Sim]                                        | 1              |
 | pais_origem                           | Não         | Numérico | Código do país de origem do servidor, de acordo com a Tabela 18                      | -              |
 | municipio_naturalidade                | Não         | Numérico | Código IBGE do município de naturalidade, de acordo com a Tabela 07                  | 8              |
 | endereco_cep                          | Não         | Caracter | CEP do endereço, preencher somente com números                                       | 8              |
 | endereco_municipio                    | Não         | Numérico | Código IBGE do município atual, de acordo com a Tabela 07                            | 8              |
 | endereco_tipo_logradouro              | Não         | Numérico | Tipo do logradouro, de acordo com a Tabela 08                                        | 2              |
 | endereco_tipo_imovel                  | Não         | Numérico | Tipo de imóvel, de acordo com a Tabela 27                                            | 2              |
 | endereco_logradouro                   | Não         | Caracter | Logradouro                                                                           | 40             |
 | endereco_bairo                        | Não         | Caracter | Bairro                                                                               | 30             |
 | endereco_complemento_logradouro       | Não         | Caracter | Complemento do logradouro                                                            | 30             |
 | endereco_numero_logradouro            | Não         | Caracter | Número do logradouro, preencher somente com números                                  | 5              |
 | telefone_ddd                          | Não         | Caracter | DDD do telefone                                                                      | 2              |
 | telefone                              | Não         | Caracter | Número do telefone, preencher somente com números                                    | 9              |
 | celular_ddd                           | Não         | Caracter | DDD do celular                                                                       | 2              |
 | celular                               | Não         | Caracter | Número do celular, preencher somente com números                                     | 9              |
 | pasep_pis_nit                         | Não         | Caracter | Número de PIS/PASEP/NIT, preencher somente com números                               | 11             |
 | cor_raca                              | Não         | Numérico | Cor/raça, de acordo com a Tabela 03                                                  | -              |
 | data_ingresso_servico_publico         | Não         | Caracter | Data de ingresso no serviço público, preencher no formato DD/MM/AAAA                 | 10             |
 | cnh                                   | Não         | Caracter | Número da CNH, preencher somente com números                                         | -              |
 | cnh_data_validade                     | Não         | Caracter | Data de validade da CNH, preencher no formato DD/MM/AAAA                             | 10             |
 | ctps                                  | Não         | Numérico | Número da CTPS, preencher somente com números                                        | 8              |
 | ctps_serie                            | Não         | Caracter | Série da CTPS                                                                        | 10             |
 | ctps_data_emissao                     | Não         | Caracter | Data de emissão da CTPS, preencher no formato DD/MM/AAAA                             | 10             |
 | titulo_eleitor_numero                 | Não         | Caracter | Número do título de eleitor, preencher somente com números                           | 14             |
 | titulo_eleitor_zona                   | Não         | Numérico | Zona do título de eleitor                                                            | -              |
 | titulo_eleitor_numero_secao_eleitoral | Não         | Numérico | Seção do título de eleitor                                                           | -              |
 | titulo_eleitor_uf_expedicao           | Não         | Numérico | Código IBGE da UF de emissão do título de eleitor, de acordo com a Tabela 08         | -              |
 | data_falecimento                      | Não         | Caracter | Data de falecimento do servidor, preencher no formato DD/MM/AAAA                     | 10             |
 | certidao_obito_termo                  | Não         | Caracter | Número do termo da certidão de óbito, preencher somente com números                  | 15             |
 | certidao_obito_livro                  | Não         | Caracter | Número do livro da certidão de óbito, preencher somente com números                  | 15             |
 | certidao_obito_folha                  | Não         | Caracter | Número da folha da certidão de óbito, preencher somente com números                  | 6              |
 | certidao_obito_data_emissao           | Não         | Caracter | Data de emissão da certidão de óbito, preencher no formato DD/MM/AAAA                | 10             |
 | cartorio_obito_cnpj                   | Não         | Caracter | CNPJ do cartório de registro do óbito, preencher somente com números                 | 8              |
 | cartorio_obito_nome                   | Não         | Caracter | Nome do cartório de registro do óbito                                                | 40             |
 | cartorio_obito_cep                    | Não         | Caracter | CEP do cartório de registro do óbito, preencher somente com números                  | 8              |
 | cartorio_obito_municipio              | Não         | Numérico | Código IBGE do município do cartório de registro do óbito, de acordo com a Tabela 07 | 8              |
 | cartorio_obito_tipo_logradouro        | Não         | Numérico | Tipo de logradouro do cartório de registro do óbito, de acordo com a Tabela 28       | 2              |
 | cartorio_obito_logradouro             | Não         | Caracter | Logradouro do cartório de registro do óbito                                          | 40             |
 | cartorio_obito_bairro                 | Não         | Caracter | Bairro do cartório de registro do óbito                                              | 30             |
 | cartorio_obito_complemento_logradouro | Não         | Caracter | Complemento do logradouro do cartório de registro do óbito                           | 30             |
 | cartorio_obito_numero_logradouro      | Não         | Caracter | Número do logradouro do cartório de registro do óbito, preencher somente com números | 5              |
