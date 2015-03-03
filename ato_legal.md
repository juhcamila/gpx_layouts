# Layout de exportação dos dados de ato legal para o GestPrev Next

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

### Atributo(s) da chave de identificação para importação de dados

* **chave  ato legal**
    * tipo_ato, numero, ano, data_publicacao, data_inicio_vigencia
