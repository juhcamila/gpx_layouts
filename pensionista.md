# Layout de exportação dos dados de pensionistas para o GestPrev Next

### Observações:

 - O arquivo deve estar em formato CSV **com header** e separado por “,”.
 - Tanto os headers quanto os valores devem estar entre "aspas duplas".
 - Os campos não podem conter caracteres especiais que não sejam acentos. Exemplo: “, ‘, ;.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente devem conter uma casa decimal. Exemplo: “100.0” ou “456.78”.
 - A coluna tamanho informa o limite máximo de caracteres aceitáveis na coluna. Não é necessário preencher o resto com espaço.

### Tabela de atributos

 | Atributo                                   | Obrigatório | Tipo     | Descrição                                                                                             | Tamanho máximo |
 | :----------------------------------------- | :---------- | :------- | :---------------------------------------------------------------------------------------------------- | -------------: |
 | nome                                       | Sim         | Caracter | Nome completo                                                                                         | 80             |
 | nome_mae                                   | Sim         | Caracter | Nome completo da mãe                                                                                  | 80             |
 | data_nascimento                            | Sim         | Data     | Data de nascimento, preencher no formato DD/MM/AAAA                                                   | 10             |
 | cpf                                        | Não         | Caracter | CPF, preencher somente com números                                                                    | 11             |
 | nome_pai                                   | Não         | Caracter | Nome completo do pai                                                                                  | 80             |
 | rg                                         | Não         | Caracter | Número do RG, preencher somente com números                                                           | 20             |
 | rg_uf_expedicao                            | Não         | Numérico | Código IBGE da UF de expedição do RG, de acordo com a Tabela 08                                       | 8              |
 | rg_orgao_emissor                           | Não         | Numérico | Código do órgão emissor do RG, de acordo com a Tabela 16                                              | -              |
 | rg_data_expedicao                          | Não         | Data     | Data de expedição do RG, preencher no formato DD/MM/AAAA                                              | 10             |
 | estado_civil                               | Não         | Numérico | Código do estado civil, de acordo com a Tabela 06                                                     | 2              |
 | email                                      | Não         | Caracter | Correio eletrônico                                                                                    | 80             |
 | tipo_sanguineo                             | Não         | Numérico | Tipo sanguíneo, de acordo com a Tabela 29                                                             | -              |
 | escolaridade                               | Não         | Numérico | Escolaridade, de acordo com a Tabela 04                                                               | -              |
 | sexo                                       | Não         | Numérico | Sexo [0: Masculino, 1: Feminino]                                                                      | 1              |
 | tipo_deficiencia                           | Não         | Numérico | Tipo de deficiência, de acordo com a Tabela 25                                                        | 1              |
 | naturalizado                               | Não         | Numérico | Se o servidor é naturalizado [0: Não, 1: Sim]                                                         | 1              |
 | pais_origem                                | Não         | Numérico | Código do país de origem do servidor, de acordo com a Tabela 18                                       | -              |
 | municipio_naturalidade                     | Não         | Numérico | Código IBGE do município de naturalidade, de acordo com a Tabela 07                                   | 8              |
 | endereco_cep                               | Não         | Caracter | CEP do endereço, preencher somente com números                                                        | 8              |
 | endereco_municipio                         | Não         | Numérico | Código IBGE do município atual, de acordo com a Tabela 07                                             | 8              |
 | endereco_tipo_logradouro                   | Não         | Numérico | Tipo do logradouro, de acordo com a Tabela 08                                                         | 2              |
 | endereco_tipo_imovel                       | Não         | Numérico | Tipo de imóvel, de acordo com a Tabela 27                                                             | 2              |
 | endereco_logradouro                        | Não         | Caracter | Logradouro                                                                                            | 40             |
 | endereco_bairo                             | Não         | Caracter | Bairro                                                                                                | 30             |
 | endereco_complemento_logradouro            | Não         | Caracter | Complemento do logradouro                                                                             | 30             |
 | endereco_numero_logradouro                 | Não         | Caracter | Número do logradouro, preencher somente com números                                                   | 5              |
 | telefone_ddd                               | Não         | Caracter | DDD do telefone                                                                                       | 2              |
 | telefone                                   | Não         | Caracter | Número do telefone, preencher somente com números                                                     | 9              |
 | celular_ddd                                | Não         | Caracter | DDD do celular                                                                                        | 2              |
 | celular                                    | Não         | Caracter | Número do celular, preencher somente com números                                                      | 9              |
 | pasep_pis_nit                              | Não         | Caracter | Número de PIS/PASEP/NIT, preencher somente com números                                                | 11             |
 | cor_raca                                   | Não         | Numérico | Cor/raça, de acordo com a Tabela 03                                                                   | -              |
 | certidao_nascimento_numero                 | Não         | Caracter | Número do termo da certidão de nascimento                                                             | 15             |
 | certidao_nascimento_livro                  | Não         | Caracter | Número do livro da certidão de nascimento                                                             | 10             |
 | certidao_nascimento_folha                  | Não         | Caracter | Número da folha da certidão de nascimento                                                             | 6              |
 | numero_matricula                           | Não         | Caracter | Matrícula                                                                                             | 20             |
 | dependencia_tipo_dependencia               | Sim         | Numérico | Tipo da dependência entre o pensionista e o servidor vinculado, de acordo com a Tabela 26             |                |
 | dependencia_fins_previdenciarios           | Não         | Caracter | Informa se a dependência será indicada para fins previdenciários [0: Não, 1: Sim]                     |                |
 | dependencia_inicio_data                    | Não         | Data     | Data de início da dependência, preencher no formato DD/MM/AAAA                                        |                |
 | dependencia_inicio_motivo                  | Não         | Numérico | Motivo de início da dependência, de acordo com a Tabela 13                                            |                |
 | dependencia_fim_data                       | Não         | Data     | Data de fim da dependência, preencher no formato DD/MM/AAAA                                           |                |
 | dependencia_fim_motivo                     | Não         | Numérico | Motivo de fim da dependência, de acordo com a Tabela 10                                               |                |
 | dependencia_fim_previsao                   | Não         | Data     | Data de previsão para fim da dependência, preencher no formato DD/MM/AAAA                             |                |
 | dependencia_descricao_outro_tipo           | Não         | Caracter | Descrição do outro tipo de dependência caso seja escolhido um valor de tipo de dependência igual a 99 | 50             |
 | dependencia_pensao_data_inicio             | Não         | Data     | Data de início da pensão adquirida pela dependência, preencher no formato DD/MM/AAAA                  |                |
 | dependencia_pensao_motivo_inicio           | Não         | Numérico | Movito de início da pensão, de acordo com a Tabela 14                                                 |                |
 | dependencia_pensao_motivo_fim              | Não         | Numérico | Movito de fim da pensão, de acordo com a Tabela 11                                                    |                |
 | dependencia_justificativa_inicio_pensao    | Não         | Caracter | Justificativa do motivo de início de pensão caso seja escolhido um valor diferente de 10              | 50             |
 | dependencia_justificativa_fim_pensao       | Não         | Caracter | Justificativa do motivo de fim de pensão caso seja escolhido um valor igual a 51 ou 99                | 50             |
 | dependencia_ato_legal_tipo_ato             | Sim         | Numérico | Tipo do ato legal, de acordo com a Tabela 23                                                          | 2              |
 | dependencia_ato_legal_numero               | Sim         | Caracter | Número do ato legal, preencher somente com números                                                    | 12             |
 | dependencia_ato_legal_ano                  | Sim         | Numérico | Ano do ato legal                                                                                      | 4              |
 | dependencia_ato_legal_data_publicacao      | Sim         | Data     | Data de publicação do ato legal, preencher no formato DD/MM/AAAA                                      | 10             |
 | dependencia_ato_legal_data_inicio_vigencia | Sim         | Data     | Data de início de vigência do ato legal, preencher no formato DD/MM/AAAA                              | 10             |
 | dependencia_ato_legal_data_revogacao       | Não         | Data     | Data de revogação do ato legal, preencher no formato DD/MM/AAAA                                       | 10             |
 | dependencia_ato_legal_resumo_ementa        | Não         | Caracter | Resumo da ementa do ato legal                                                                         | 100            |
 | dependencia_ato_legal_ementa               | Não         | Caracter | Ementa do ato legal                                                                                   | 1000           |
 | servidor_vinculado_nome                    | Sim         | Caracter | Nome completo do servidor vinculado                                                                   | 80             |
 | servidor_vinculado_nome_mae                | Não         | Caracter | Nome completo da mãe do servidor vinculado                                                            | 80             |
 | servidor_vinculado_data_nascimento         | Não         | Data     | Data de nascimento do servidor vinculado , preencher no formato DD/MM/AAAA                            | 10             |
 | servidor_vinculado_cpf                     | Não         | Caracter | CPF, preencher somente com números do servidor vinculado                                              | 11             |
 | servidor_vinculado_pasep_pis_nit           | Não         | Caracter | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                          | 11             |
