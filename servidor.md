# Layout de exportação dos dados de servidores para o Gestprev

### Observações:

 - O arquivo deve estar em formato CSV com header e separado por “,”.
 - Tanto os headers quanto os valores devem estar entre "aspas duplas".
 - Os campos não podem conter caracteres especiais que não sejam acentos. Exemplo: “, ‘, ;.
 - Campos em negrito são obrigatórios e devem ser preenchidos.
 - Se o campo não for string, o formato em que deverá ser preenchido está entre “[“ e “]” na descrição.
 - Deve haver uma coluna para cada campo do arquivo, mesmo que o campo não seja preenchido.
 - Campos de valores obrigatoriamente devem conter uma casa decimal. Exemplo: “100.0” ou “456.78”.

### Tabela de atributos

Atributo | Tipo | Descrição | Tamanho
:------ | :--: | :------- | :-------:
nome | string | Nome do servidor | 80
rg | string | Número da RG do servidor | 20
nascimento | string | Data de nascimento do servidor | 10
estado_civil | integer | Estado civil do servidor, de acordo com tabela ## | 2
nome_pai | string | Nome do pai do servidor | 80
nome_mae | string | Nome da mãe do servidor | 80
email | string | Correio eletrônico do servidor | 80
logradouro | string | Logradouro do servidor | 40
numero_logradouro | string | Número do logradouro do servidor | 5
bairo | string | Bairro do servidor | 30
data_expedicao_rg | date | Data de expedição do RG | -
tipo_sanguineo | integer | Tipo sanguíneo do servidor, de acordo com tabela ## | -
escolaridade | integer | Escolaridade do servidor, de acordo com tabela ## | -
tipo_logradouro | integer | Tipo do logradouro do servidor, de acordo com tabela ## | 2
sexo | integer | Sexo do servidor. [0: Masculino, 1: Feminino] | 1
deficiente | integer | Se o servidor é deficiente. [0: Não, 1: Sim] | 1
naturalizado | integer | Se o servidor é naturalizado. [0: Não, 1: Sim] | 1
municipio | integer | Código IBGE do município atual do servidor, de acordo com referência ## | 8
uf_expedicao_rg | integer | Código IBGE da UF de expedição do RG do servidor, de acordo com referência ## | 8
orgao_emissor_identidade | integer | Código do órgão emissor do RG | -
complemento_logradouro | string | Complemento do logradouro do servidor. | 30
pais | integer | Código do pais do servidor. De acordo com referência ## | -
municipio_naturalidade | integer | Código IBGE do Município de naturalidade do servidor. | 8
ddd_telefone | string | DDD do telefone do servidor. | 2
telefone | string | Número do telefone do servidor. | 9
ddd_celular | string | DDD do celular do servidor. | 2
celular | string | Número do celular do servidor. | 9
cep | string | CEP do servidor | 8
pasep_pis_nit | string | Número de PIS/PASEP do servidor | 11
cpf | string | CPF do servidor. | 11
cor_raca | integer | Cor/raça do servidor. De acordo com referência ## | -
cnh | string | Número da CNH do servidor | -
data_validade_cnh | string | #descricao | -
instituidor | integer | #descricao | 1
ctps | integer | #descricao | 8
ctps_serie | string | #descricao | 10
ctps_emissao | string | #descricao | 10
numero_titulo_eleitor | string | #descricao | 14
zona_titulo_eleitor | integer | #descricao | -
numero_secao_eleitoral | integer | #descricao | -
data_ingresso_servico_publico | string | #descricao | 10
documento_ingresso_servico_publico | string | #descricao | 50
data_falecimento | string | #descricao | 10
termo_certidao_obito | string | #descricao | 15
livro_certidao_obito | string | #descricao | 15
folha_certidao_obito | string | #descricao | 6
emissao_certidao_obito | string | #descricao | -
justificativa_obito | string | #descricao | 200
uf_expedicao_id_ibge | integer | #descricao | -

