# Layout de exportação dos dados de servidores para o GestPrev Next

### Observações:

 - O arquivo deve estar em formato CSV **com header** e separado por “,”.
 - Tanto os headers quanto os valores devem estar entre "aspas duplas", mesmo que os valores estejam em branco.
 - Os campos não devem conter caracteres especiais que não sejam acentos. Exemplo: “, ‘, ;.
 - Campos em negrito são obrigatórios e devem ser preenchidos.
 - Se o campo não for string, o formato em que deverá ser preenchido está entre “[“ e “]” na descrição.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente devem conter uma casa decimal. Exemplo: “100.0” ou “456.78”.

### Tabela de atributos

   | Atributo               | Obrigatório | Tipo     | Descrição                                                             | Tamanho  |
   | :-------               | :---------- | :---     | :--------                                                             | -------: |
   | nome                   | Sim         | Caracter | Nome do órgão                                                         | 100      |
   | sigla                  | Não         | Caracter | Sigla do órgão                                                        | 10       |
   | razao_social           | Não         | Caracter | Razão social do órgão                                                 | 100      |
   | cnpj                   | Não         | Caracter | Número do CNPJ do Órgão. Preencher apenas com números                 | 14       |
   | cep                    | Não         | Caracter | CEP do endereço do órgão. Preencher apenas com números                | 8        |
   | municipio              | Não         | Numérico | Código IBGE do município do endereço do órgão. Ver tabela anexa       | 6        |
   | tipo_logradouro        | Não         | Numérico | Tipo de logradouro do endereço. Ver tabela anexa                      | 2        |
   | logradouro             | Não         | Caracter | Logradouro do órgão                                                   | 40       |
   | bairro                 | Não         | Caracter | Bairro do endereço do órgão                                           | 30       |
   | complemento_logradouro | Não         | Caracter | Complemento do endereço do órgão                                      | 30       |
   | numero_logradouro      | Não         | Caracter | Número do endereço do órgão                                           | 5        |
   | email                  | Não         | Caracter | Correio eletrônico do órgão                                           | 80       |
   | site                   | Não         | Caracter | Site do órgão                                                         | 40       |
   | ddd_telefone           | Não         | Caracter | Número do DDD do telefone fixo do órgão. Preencher apenas com números | 2        |
   | telefone               | Não         | Caracter | Número do telefone fixo do órgão. Preencher apenas com números        | 9        |
   | ddd_fax                | Não         | Caracter | Número do DDD do fax do órgão. Preencher apenas com números           | 2        |
   | fax                    | Não         | Caracter | Número do fax do órgão. Preencher apenas com números                  | 9        |
   | poder                  | Sim         | Numérico | Poder do órgão. Ver tabela anexa                                      | -        |
   | esfera                 | Não         | Numérico | Esfera do órgão. Ver tabela anexa                                     | -        |
   | natureza_juridica      | Não         | Numérico | Natureza Jurídica do órgão. Ver tabela anexa                          | -        |
