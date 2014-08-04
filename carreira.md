# Layout de exportação dos dados de carreira para o GestPrev Next

### Observações:

 - O arquivo deve estar em formato CSV **com header** e separado por “,”.
 - Tanto os headers quanto os valores devem estar entre "aspas duplas", mesmo que os valores estejam em branco.
 - Os campos não devem conter caracteres especiais que não sejam acentos. Exemplo: “, ‘, ;.
 - Campos em negrito são obrigatórios e devem ser preenchidos.
 - Se o campo não for string, o formato em que deverá ser preenchido está entre “[“ e “]” na descrição.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente devem conter uma casa decimal. Exemplo: “100.0” ou “456.78”.

### Tabela de atributos

 | Atributo                                   | Obrigatório | Tipo     | Descrição                                                                                           | Tamanho máximo |
 | :----------------------------------------- | :---------- | :------- | :-------------------------------------------------------------------------------------------------- | -------------: |
 | nome                                       | Sim         | Caracter | Nome da carreira                                                                                    | 60             |
 | codigo_origem                              | Não         | Caracter | Código de origem da carreira                                                                        | 6              |
 | data_criacao                               | Não         | Data     | Data da criação da carreira, preencher no formato DD/MM/AAAA                                        | 10             |
 | data_extincao                              | Não         | Data     | Data da extinção da carreira, preencher no formato DD/MM/AAAA                                       | 10             |
 | orgao_nome_orgao                           | Sim         | Caracter | Nome do órgão vinculado à carreira                                                                  | 100            |
 | orgao_poder                                | Sim         | Numérico | Poder do órgão vinculado à carreira, de acordo com a Tabela 19                                      | 1              |
 | ato_legal_criacao_tipo_ato                 | Sim         | Numérico | Tipo do ato legal de criação da carreira, de acordo com a Tabela 23                                 | 2              |
 | ato_legal_criacao_numero                   | Sim         | Caracter | Número do ato legal de criaçao da carreira, preencher somente com números                           | 12             |
 | ato_legal_criacao_ano                      | Sim         | Numérico | Ano do ato legal de criação da carreira                                                             | 4              |
 | ato_legal_criacao_data_publicacao          | Sim         | Data     | Data de publicação do ato legal de criação da carreira, preencher no formato DD/MM/AAAA             | 10             |
 | ato_legal_criacao_data_inicio_vigencia     | Sim         | Data     | Data de início de vigência do ato legal de criação da carreira, preencher no formato DD/MM/AAAA     | 10             |
 | ato_legal_criacao_data_revogacao           | Não         | Data     | Data de revogação do ato legal de criação da carreira, preencher no formato DD/MM/AAAA              | 10             |
 | ato_legal_criacao_resumo_ementa            | Não         | Caracter | Resumo da ementa do ato legal de criação da carreira                                                | 100            |
 | ato_legal_criacao_ementa                   | Não         | Caracter | Ementa do ato legal de criação da carreira                                                          | 1000           |
 | ato_legal_remuneracao_tipo_ato             | Sim         | Numérico | Tipo do ato legal da remuneração da carreira, de acordo com a Tabela 23                             | 2              |
 | ato_legal_remuneracao_numero               | Sim         | Caracter | Número do ato legal da remuneração da carreira, preencher somente com números                       | 12             |
 | ato_legal_remuneracao_ano                  | Sim         | Numérico | Ano do ato legal da remuneração da carreira                                                         | 4              |
 | ato_legal_remuneracao_data_publicacao      | Sim         | Data     | Data de publicação do ato legal da remuneração da carreira, preencher no formato DD/MM/AAAA         | 10             |
 | ato_legal_remuneracao_data_inicio_vigencia | Sim         | Data     | Data de início de vigência do ato legal da remuneração da carreira, preencher no formato DD/MM/AAAA | 10             |
 | ato_legal_remuneracao_data_revogacao       | Não         | Data     | Data de revogação do ato legal da remuneração da carreira, preencher no formato DD/MM/AAAA          | 10             |
 | ato_legal_remuneracao_resumo_ementa        | Não         | Caracter | Resumo da ementa do ato legal da remuneração da carreira                                            | 100            |
 | ato_legal_remuneracao_ementa               | Não         | Caracter | Ementa do ato legal da remuneração da carreira                                                      | 1000           |