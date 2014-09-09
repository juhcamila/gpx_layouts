# Layouts de exportação dos dados para o GestPrev Next

Este repositório reúne os layouts que devem ser disponibilizados para a migração de dados externos para o GestPrev Next.

Os layouts contemplam de forma compatível todos os campos essenciais e obrigatórios do sistema SIPREV Gestão.

## Observações

Os arquivos devem respeitar algumas regras de formatação para serem recebidos pelo sistema:

 - Cada arquivo deve estar em formato CSV **com header** e separado por “`,`” (vírgula).
 - Cada arquivo deve possuir a extensão ".csv".
 - Tanto os headers quanto os valores devem estar entre `""` (aspas duplas), mesmo que os valores estejam em branco. Não deverá haver espaço em branco entre as aspas e o separador de coluna.
 - Os campos não devem conter caracteres especiais que não sejam acentos. Por exemplo: “`,` `‘`, `;`".
 - A coluna tamanho máximo indica a quantidade máxima de caracteres da coluna. Não é necessário preencher o resto com espaços.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente **devem conter uma casa decimal**. Por exemplo: “100.0” ou “456.78”.

Exemplo de arquivo no formato CSV válido para importação:

```
"nome","email","idade"
"Francisco","xicinho@exemplo.com","32"
"Maria","maria@exemplo.com","27"
```

Exemplo de arquivo no formato CSV inválido para importação:

```
"nome", "email", "idade"
"Francisco", "xicinho@exemplo.com", 32
Maria, "maria@exemplo.com", 27
```

(espaços entre os valores e o separador, colunas sem quotes [`""`])

### Sobre os Atos Legais

Atos legais estão associados a vários tipos de registros, tais como órgãos, dependentes, carreiras, etc.

Em cada layout, os atributos `tipo`, `número,`, `ano`, `data publicação` e `data início vigência` estão marcados como obrigatórios.

É importante notar que **a ausência do Ato Legal não impede a criação do registro**, e estes atributos apenas são obrigatórios caso o Ato Legal esteja presente.


### Registros associados à um servidor

Para associar um servidor à um registro, os layouts aceitam os seguintes campos referentes ao servidor a ser associado: `nome`, `nome mãe`, `data de nascimento`, `CPF`, `PIS/PASEP/NIT`.

A combinação de atributos a seguir será usada como chave para buscar um servidor, em ordem de precedência:

* PIS/PASEP/NIT ou;
* CPF ou;
* Nome, nome da mãe, data de nascimento.

Caso nenhum servidor seja encontrado usando as chaves acima, o registro não será importado.

### Regras para importação dos dados

Cada linha presente no arquivo CSV recebido(exceto é claro a linha que representa o cabeçalho do formato CSV) será utilizada para a operação de inclusão e/ou alteração de dados no sistema. Para realizar tais operações, é necessário que sejam informados todos os atributos que compõe uma chave de identificação única no sistema.

Cada arquivo de layout possui a combinação e descrição de quais atributos podem ser utilizados para compor a chave de identificação.

Durante o processo de importação de dados, nosso sistema identifica a chave de identificação e realiza a operação de inclusão. No caso de já existir os dados no sistema, então procede-se a operação de alteração dos dados, exceto para os atributos que compõe a chave de identificação única.

Caso haja no arquivo de importação linhas com chaves de identificação repetidas, os valores dos demais atributos a serem incluídos ou alterados no sistema, serão sempre os valores da última linha encontrada no arquivo para a chave em questão.

A alteração dos atributos que compõe uma chave de identificação única no sistema poderá ser realizada somente através do sistema Gestprev Next.

No caso de uma chave de identificação única não ser informada ou ser informada incorretamente ou ser informada com atributos incompletos, a operação de inclusão e/ou alteração não poderá ser realizada.
