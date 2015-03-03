# Layout de exportação dos dados de órgão para o GestPrev Next

### Tabela de atributos

    | Atributo                         | Obrigatório | Tipo     | Descrição                                                                 | Tamanho máximo |
    | :------------------------------- | :---------- | :------- | :------------------------------------------------------------------------ | -------------: |
    | nome                             | Sim         | Caracter | Nome do órgão                                                             | 100            |
    | sigla                            | Não         | Caracter | Sigla do órgão                                                            | 10             |
    | razao_social                     | Não         | Caracter | Razão social do órgão                                                     | 100            |
    | cnpj                             | Não         | Caracter | Número do CNPJ do órgão, preencher apenas com números                     | 14             |
    | endereco_cep                     | Não         | Caracter | CEP do endereço do órgão, preencher apenas com números                    | 8              |
    | endereco_municipio               | Não         | Numérico | Código IBGE do município do endereço do órgão, de acordo com a Tabela 07  | 6              |
    | endereco_tipo_logradouro         | Não         | Numérico | Tipo de logradouro do endereço, de acordo com a Tabela 28                 | 3              |
    | endereco_logradouro              | Não         | Caracter | Logradouro do órgão                                                       | 40             |
    | endereco_bairro                  | Não         | Caracter | Bairro do endereço do órgão                                               | 30             |
    | endereco_complemento_logradouro  | Não         | Caracter | Complemento do endereço do órgão                                          | 30             |
    | endereco_numero_logradouro       | Não         | Caracter | Número do endereço do órgão                                               | 5              |
    | email                            | Não         | Caracter | Correio eletrônico do órgão                                               | 80             |
    | site                             | Não         | Caracter | Site do órgão                                                             | 40             |
    | telefone_ddd                     | Não         | Caracter | Número do DDD do telefone fixo do órgão, preencher apenas com números     | 2              |
    | telefone                         | Não         | Caracter | Número do telefone fixo do órgão, preencher apenas com números            | 9              |
    | fax_ddd                          | Não         | Caracter | Número do DDD do fax do órgão, preencher apenas com números               | 2              |
    | fax                              | Não         | Caracter | Número do fax do órgão, preencher apenas com números                      | 9              |
    | poder                            | Sim         | Numérico | Poder do órgão, de acordo com a Tabela 19                                 | 1              |
    | esfera                           | Não         | Numérico | Esfera do órgão, de acordo com a Tabela 05                                | 1              |
    | natureza_juridica                | Não         | Numérico | Natureza Jurídica do órgão, de acordo com a Tabela 15                     | 2              |
    | ato_legal_tipo_ato               | Sim\*       | Numérico | Tipo do ato legal, de acordo com a Tabela 23                              | 2              |
    | ato_legal_numero                 | Sim\*       | Caracter | Número do ato legal, preencher somente com números                        | 12             |
    | ato_legal_ano                    | Sim\*       | Numérico | Ano do ato legal                                                          | 4              |
    | ato_legal_data_publicacao        | Sim\*       | Data     | Data de publicação do ato legal, preencher no formato DD/MM/AAAA          | 10             |
    | ato_legal_data_inicio_vigencia   | Sim\*       | Data     | Data de início de vigência do ato legal, preencher no formato DD/MM/AAAA  | 10             |
    | ato_legal_data_revogacao         | Não         | Data     | Data de revogação do ato legal, preencher no formato DD/MM/AAAA           | 10             |
    | ato_legal_resumo_ementa          | Não         | Caracter | Resumo da ementa do ato legal                                             | 100            |
    | ato_legal_ementa                 | Não         | Caracter | Ementa do ato legal                                                       | 1000           |

\* Este campo é obrigatório apenas se o Ato Legal estiver presente.

---

### Atributo(s) da chave de identificação para importação de dados

* **chave órgão**
    * nome e poder

* **chave ato legal**
    * ato_legal_tipo_ato, ato_legal_numero, ato_legal_ano
