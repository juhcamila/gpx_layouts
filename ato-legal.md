# Layout de exportação dos dados de ato legal para o GestPrev Next

### Observações:

 - O arquivo deve estar em formato CSV **com header** e separado por “,”.
 - Tanto os headers quanto os valores devem estar entre "aspas duplas", mesmo que os valores estejam em branco.
 - Os campos não devem conter caracteres especiais que não sejam acentos. Exemplo: “, ‘, ;.
 - Campos em negrito são obrigatórios e devem ser preenchidos.
 - Se o campo não for string, o formato em que deverá ser preenchido está entre “[“ e “]” na descrição.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente devem conter uma casa decimal. Exemplo: “100.0” ou “456.78”.

### Tabela de atributos

 | Atributo              | Obrigatório | Tipo      | Descrição                                                                 | Tamanho máximo  |
 | :-------------------- | :---------- | :-------- | :------------------------------------------------------------------------ | --------------: |
 | tipo_ato              | Sim         | Numérico  | Tipo do ato legal, de acordo com a Tabela 23                              | 2               |
 | numero                | Sim         | Caracter  | Número do ato legal, preencher somente com números                        | 12              |
 | ano                   | Sim         | Numérico  | Ano do ato legal                                                          | 4               |
 | data_publicacao       | Sim         | Data      | Data de publicação do ato legal, preencher no formato DD/MM/AAAA          | 10              |
 | data_inicio_vigencia  | Sim         | Data      | Data de início de vigência do ato legal, preencher no formato DD/MM/AAAA  | 10              |
 | data_revogacao        | Não         | Data      | Data de revogação do ato legal, preencher no formato DD/MM/AAAA           | 10              |
 | resumo_ementa         | Não         | Caracter  | Resumo da ementa do ato legal                                             | 100             |
 | ementa                | Não         | Caracter  | Ementa do ato legal                                                       | 1000            |
