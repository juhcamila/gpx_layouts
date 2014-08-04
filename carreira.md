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

  | Atributo      | Obrigatório | Tipo     | Descrição                                                                         | Tamanho  |
  | :-------      | :---------- | :---     | :--------                                                                         | -------: |
  | nome          | Sim         | Caracter | Nome da carreira                                                                  | 60       |
  | codigo_origem | Não         | Caracter | Código de origem da carreira                                                      | 6        |
  | data_criacao  | Não         | Caracter | Data da criação da carreira. Preencher no formato preencher no formato DD/MM/AAAA | 10       |
  | data_extincao | Não         | Caracter | Data da extinção da carreira. Preencher no formato DD/MM/AAAA                     | 10       |
  | nome_orgao    | Sim         | Caracter | Nome do órgão vinculado à carreira                                                | 100      |
  | poder         | Sim         | Numérico | Poder do órgão vinculado à carreira. Ver tabela anexa                             | 1        |
