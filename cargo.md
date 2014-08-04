# Layout de exportação dos dados de cargo para o GestPrev Next

### Observações:

 - O arquivo deve estar em formato CSV **com header** e separado por “,”.
 - Tanto os headers quanto os valores devem estar entre "aspas duplas", mesmo que os valores estejam em branco.
 - Os campos não devem conter caracteres especiais que não sejam acentos. Exemplo: “, ‘, ;.
 - Campos em negrito são obrigatórios e devem ser preenchidos.
 - Se o campo não for string, o formato em que deverá ser preenchido está entre “[“ e “]” na descrição.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente devem conter uma casa decimal. Exemplo: “100.0” ou “456.78”.

### Tabela de atributos

| Atributo               | Obrigatório | Tipo     | Descrição                                                               | Tamanho  | Decimais |
| :-------               | :---------- | :---     | :--------                                                               | -------: | -        |
| nome                   | Sim         | Caracter | Nome do cargo                                                           | 60       | -        |
| codigo_origem          | Não         | Caracter | Código de origem da carreira                                            | 6        | -        |
| data_criacao           | Não         | Caracter | Data da criação da carreira. Preencher no formato DD/MM/AAAA            | 10       | -        |
| data_extincao          | Não         | Caracter | Data da extinção da carreira. Preencher no formato DD/MM/AAAA           | 10       | -        |
| cargo_acumulacao       | Sim         | Numérico | Cargo com acumulação, de acordo com a Tabela 32                         | 1        | -        |
| contagem_especial      | Sim         | Numérico | Cargo com contagem de tempo especial, de acordo com a Tabela 02         | 1        | -        |
| tecnico_cientifico     | Sim         | Numérico | Cargo técnico científico. [0: Não, 1: Sim]                              | 1        | -        |
| remuneracao_inicial    | Não         | Numérico | Valor da remuneração inicial do cargo                                   | 8        | 2        |
| remuneracao_final      | Não         | Numérico | Valor da remuneração final do cargo                                     | 8        | 2        |
| aposentadoria_especial | Sim         | Numérico | Cargo tem aposentadoria especial. [0: Não, 1: Sim]                      | 1        | -        |
| dedicacao_exclusiva    | Sim         | Numérico | Cargo com dedicação exclusiva. [0: Não, 1: Sim]                         | 1        | -        |
| nome_carreira          | Sim         | Caracter | Nome da carreira na qual o cargo está vinculado                         | 60       | -        |
| nome_orgao             | Sim         | Caracter | Nome do órgão vinculado à carreira do cargo                             | 100      | -        |
| poder                  | Sim         | Numérico | Poder do órgão vinculado à carreira do cargo, de acordo com a Tabela 19 | 1        | -        |
