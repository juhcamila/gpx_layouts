# Layout de exportação dos dados de dependentes para o GestPrev Next

### Tabela de atributos

 | Atributo                                            | Obrigatório | Tipo     | Descrição                                                                                                    | Tamanho máximo |
 | :-------------------------------------------------- | :---------- | :------- | :----------------------------------------------------------------------------------------------------        | -------------: |
 | nome                                                | Sim         | Caracter | Nome completo                                                                                                | 80             |
 | nome_mae                                            | Sim         | Caracter | Nome completo da mãe                                                                                         | 80             |
 | data_nascimento                                     | Sim         | Data     | Data de nascimento, preencher no formato DD/MM/AAAA                                                          | 10             |
 | cpf                                                 | Não         | Caracter | CPF, preencher somente com números                                                                           | 11             |
 | nome_pai                                            | Não         | Caracter | Nome completo do pai                                                                                         | 80             |
 | rg                                                  | Não         | Caracter | Número do RG, preencher somente com números                                                                  | 20             |
 | rg_uf_expedicao                                     | Não         | Numérico | Código IBGE da UF de expedição do RG, de acordo com a Tabela 08                                              | 8              |
 | rg_orgao_emissor                                    | Não         | Numérico | Código do órgão emissor do RG, de acordo com a Tabela 16                                                     | 2              |
 | rg_data_expedicao                                   | Não         | Data     | Data de expedição do RG, preencher no formato DD/MM/AAAA                                                     | 10             |
 | estado_civil                                        | Não         | Numérico | Código do estado civil, de acordo com a Tabela 06                                                            | 2              |
 | email                                               | Não         | Caracter | Correio eletrônico                                                                                           | 80             |
 | tipo_sanguineo                                      | Não         | Numérico | Tipo sanguíneo, de acordo com a Tabela 29                                                                    | 1              |
 | escolaridade_nivel                                  | Não         | Numérico | Escolaridade, de acordo com a Tabela 04                                                                      | -              |
 | escolaridade_nome_curso                             | Não         | Caracter | Nome do curso acadêmico                                                                                      | 100            |
 | escolaridade_nome_instituicao                       | Não         | Caracter | Nome da instituição do curso acadêmico                                                                       | 100            |
 | escolaridade_ano_conclusao                          | Não         | Data     | Ano de conclusão do curso acadêmico                                                                          | 4              |
 | sexo                                                | Não         | Numérico | Sexo [0: Masculino, 1: Feminino]                                                                             | 1              |
 | tipo_deficiencia                                    | Não         | Numérico | Tipo de deficiência, de acordo com a Tabela 25                                                               | 1              |
 | pais_origem                                         | Não         | Numérico | Código do país de origem do servidor, de acordo com a Tabela 18                                              | 3              |
 | municipio_naturalidade                              | Não         | Numérico | Código IBGE do município de naturalidade, de acordo com a Tabela 07                                          | 8              |
 | endereco_cep                                        | Não         | Caracter | CEP do endereço, preencher somente com números                                                               | 8              |
 | endereco_municipio                                  | Não         | Numérico | Código IBGE do município atual, de acordo com a Tabela 07                                                    | 8              |
 | endereco_logradouro_tipo                            | Não         | Numérico | Tipo do logradouro, de acordo com a Tabela 08                                                                | 2              |
 | endereco_tipo_imovel                                | Não         | Numérico | Tipo de imóvel, de acordo com a Tabela 27                                                                    | 2              |
 | endereco_bairro                                     | Não         | Caracter | Bairro                                                                                                       | 30             |
 | endereco_logradouro                                 | Não         | Caracter | Logradouro                                                                                                   | 40             |
 | endereco_logradouro_complemento                     | Não         | Caracter | Complemento do logradouro                                                                                    | 30             |
 | endereco_logradouro_numero                          | Não         | Caracter | Número do logradouro, preencher somente com números                                                          | 5              |
 | telefone_ddd                                        | Não         | Caracter | DDD do telefone                                                                                              | 2              |
 | telefone                                            | Não         | Caracter | Número do telefone, preencher somente com números                                                            | 9              |
 | celular_ddd                                         | Não         | Caracter | DDD do celular                                                                                               | 2              |
 | celular                                             | Não         | Caracter | Número do celular, preencher somente com números                                                             | 9              |
 | pasep_pis_nit                                       | Não         | Caracter | Número de PIS/PASEP/NIT, preencher somente com números                                                       | 11             |
 | cor_raca                                            | Não         | Numérico | Cor/raça, de acordo com a Tabela 03                                                                          | 1              |
 | certidao_nascimento_numero                          | Não         | Caracter | Número do termo da certidão de nascimento                                                                    | 15             |
 | certidao_nascimento_livro                           | Não         | Caracter | Número do livro da certidão de nascimento                                                                    | 10             |
 | certidao_nascimento_folha                           | Não         | Caracter | Número da folha da certidão de nascimento                                                                    | 6              |
 | estrangeiro_naturalizado                            | Não         | Numérico | Se o servidor é naturalizado, para nacionalidade diferente de Brasileira. [0: Não, 1: Sim]                   | 1              |
 | estrangeiro_visto_permanente                        | Não         | Numérico | Visto permanente para nacionalidade diferente de Brasileira. [0: Não, 1: Sim]                                | 1              |
 | estrangeiro_data_chegada_brasil                     | Não         | Data     | Data de chegada ao Brasil para nacionalidade diferente de Brasileira, preencher no formato DD/MM/AAAA        | 10             |
 | estrangeiro_rg                                      | Não         | Caracter | Número do RGE, para nacionalidade diferente de Brasileira                                                    | 20             |
 | estrangeiro_rg_orgao_emissor                        | Não         | Caracter | Preencher com o nome do órgão expedição/emissor do RGE, para nacionalidade diferente de Brasileira           | -              |
 | estrangeiro_rg_uf_expedicao                         | Não         | Numérico | Código IBGE da UF de expedição do RGE, de acordo com a Tabela 08, para nacionalidade diferente de Brasileira | 8              |
 | estrangeiro_rg_data_emissao                         | Não         | Data     | Data de emissão do RGE, preencher no formato DD/MM/AAAA, para nacionalidade diferente de Brasileira          | 10             |
 | dependencia_tipo_dependencia                        | Sim         | Numérico | Tipo da dependência entre o dependente e o servidor vinculado, de acordo com a Tabela 26                     | 2              |
 | dependencia_fins_previdenciarios                    | Não         | Caracter | Informa se a dependência será indicada para fins previdenciários [0: Não, 1: Sim]                            | 1              |
 | dependencia_inicio_data                             | Não         | Data     | Data de início da dependência, preencher no formato DD/MM/AAAA                                               | 10             |
 | dependencia_inicio_motivo                           | Não         | Numérico | Motivo de início da dependência, de acordo com a Tabela 13                                                   | 2              |
 | dependencia_fim_data                                | Não         | Data     | Data de fim da dependência, preencher no formato DD/MM/AAAA                                                  | 10             |
 | dependencia_fim_motivo                              | Não         | Numérico | Motivo de fim da dependência, de acordo com a Tabela 10                                                      | 2              |
 | dependencia_fim_previsao                            | Não         | Data     | Data de previsão para fim da dependência, preencher no formato DD/MM/AAAA                                    | 10             |
 | dependencia_descricao_outro_tipo                    | Não         | Caracter | Descrição do outro tipo de dependência caso seja escolhido um valor de tipo de dependência igual a 99        | 50             |
 | dependencia_pensao_data_inicio                      | Não         | Data     | Data de início da pensão adquirida pela dependência, preencher no formato DD/MM/AAAA                         | 10             |
 | dependencia_pensao_motivo_inicio                    | Não         | Numérico | Movito de início da pensão, de acordo com a Tabela 14                                                        | 2              |
 | dependencia_pensao_motivo_fim                       | Não         | Numérico | Movito de fim da pensão, de acordo com a Tabela 11                                                           | 2              |
 | dependencia_justificativa_inicio_pensao             | Não         | Caracter | Justificativa do motivo de início de pensão caso seja escolhido um valor diferente de 10                     | 50             |
 | dependencia_justificativa_fim_pensao                | Não         | Caracter | Justificativa do motivo de fim de pensão caso seja escolhido um valor igual a 51 ou 99                       | 50             |
 | dependencia_ato_legal_tipo_ato                      | Sim\*       | Numérico | Tipo do ato legal, de acordo com a Tabela 23                                                                 | 2              |
 | dependencia_ato_legal_numero                        | Sim\*       | Caracter | Número do ato legal, preencher somente com números                                                           | 12             |
 | dependencia_ato_legal_ano                           | Sim\*       | Numérico | Ano do ato legal                                                                                             | 4              |
 | dependencia_ato_legal_data_publicacao               | Sim\*       | Data     | Data de publicação do ato legal, preencher no formato DD/MM/AAAA                                             | 10             |
 | dependencia_ato_legal_data_inicio_vigencia          | Sim\*       | Data     | Data de início de vigência do ato legal, preencher no formato DD/MM/AAAA                                     | 10             |
 | dependencia_ato_legal_data_revogacao                | Não         | Data     | Data de revogação do ato legal, preencher no formato DD/MM/AAAA                                              | 10             |
 | dependencia_ato_legal_resumo_ementa                 | Não         | Caracter | Resumo da ementa do ato legal                                                                                | 100            |
 | dependencia_ato_legal_ementa                        | Não         | Caracter | Ementa do ato legal                                                                                          | 1000           |
 | servidor_vinculado_nome                             | Sim         | Caracter | Nome completo do servidor vinculado                                                                          | 80             |
 | servidor_vinculado_nome_mae                         | Não         | Caracter | Nome completo da mãe do servidor vinculado                                                                   | 80             |
 | servidor_vinculado_data_nascimento                  | Não         | Data     | Data de nascimento do servidor vinculado , preencher no formato DD/MM/AAAA                                   | 10             |
 | servidor_vinculado_cpf                              | Não         | Caracter | CPF, preencher somente com números do servidor vinculado                                                     | 11             |
 | servidor_vinculado_pasep_pis_nit                    | Não         | Caracter | Número de PIS/PASEP/NIT do servidor vinculado, preencher somente com números                                 | 11             |
 | representatividade_tipo                             | Sim\*\*     | Numérico | Tipo da representatividade do servidor para com seu representante legal, de acordo com a Tabela 36           | 1              |
 | representatividade_data_inicio                      | Não\*\*\*   | Data     | Data de início da representatividade, preencher no formato DD/MM/AAAA                                        | 10             |
 | representatividade_data_termino_previsto            | Não\*\*\*\* | Data     | Data de término previsto da representatividade, preencher no formato DD/MM/AAAA                              | 10             |
 | representante_legal_nome                            | Sim\*\*     | Caracter | Nome do representante legal                                                                                  | 80             |
 | representante_legal_cpf                             | Sim\*\*     | Caracter | CPF do representante legal, preencher somente com números                                                    | 11             |
 | representante_legal_rg                              | Sim\*\*     | Caracter | RG do representante legal                                                                                    | 20             |
 | representante_legal_rg_orgao_expedidor              | Não         | Numérico | Código do órgão expedidor do RG, de acordo com a Tabela 16                                                   | -              |
 | representante_legal_rg_uf_expedicao                 | Não         | Caracter | Código IBGE da UF de expedição do RG do representante legal, de acordo com a Tabela 08                       | 8              |
 | representante_legal_rg_data_emissao                 | Não         | Data     | Data de emissão do RG do representante legal, preencher no formato DD/MM/AAAA                                | 10             |
 | representante_legal_data_nascimento                 | Sim\*\*     | Data     | Data de nascimento do representante legal, preencher no formato DD/MM/AAAA                                   | 10             |
 | representante_legal_sexo                            | Sim\*\*     | Numérico | Sexo do representante legal. [0: Masculino, 1: Feminino]                                                     | 1              |
 | representante_legal_endereco_cep                    | Não         | Caracter | CEP do endereço do representante legal, preencher somente com números                                        | 8              |
 | representante_legal_endereco_municipio              | Não         | Numérico | Código IBGE do município do representante legal, de acordo com a Tabela 07                                   | 8              |
 | representante_legal_endereco_logradouro_tipo        | Não         | Numérico | Tipo do logradouro do representante legal, de acordo com a Tabela 08                                         | 2              |
 | representante_legal_endereco_tipo_imovel            | Não         | Numérico | Tipo de imóvel do representante legal, de acordo com a Tabela 27                                             | 2              |
 | representante_legal_endereco_bairro                 | Não         | Caracter | Bairro do representante legal                                                                                | 30             |
 | representante_legal_endereco_logradouro             | Não         | Caracter | Logradouro do representante legal                                                                            | 40             |
 | representante_legal_endereco_logradouro_complemento | Não         | Caracter | Complemento do logradouro do representante legal                                                             | 30             |
 | representante_legal_endereco_logradouro_numero      | Não         | Caracter | Número do logradouro do representante legal, preencher somente com números                                   | 5              |
 | representante_legal_telefone_ddd                    | Não         | Caracter | DDD do telefone do representante legal                                                                       | 2              |
 | representante_legal_telefone                        | Não         | Caracter | Número do telefone do representante legal, preencher somente com números                                     | 9              |
 | representante_legal_celular_ddd                     | Não         | Caracter | DDD do celular do representante legal                                                                        | 2              |
 | representante_legal_celular                         | Não         | Caracter | Número do celular do representante legal, preencher somente com números                                      | 9              |
 | representante_legal_email                           | Não         | Caracter | Correio eletrônico                                                                                           | 80             |
 | assistencia_saude_rede_atendimento                  | Não         | Numérico | Tipo da rede de atendimento. [0: Pública, 1: Privada]                                                        | 1              |
 | assistencia_saude_plano_operadora                   | Não         | Caracter | Nome da operadora do plano de Saúde                                                                          | 100            |
 | assistencia_saude_plano_nome                        | Não         | Caracter | Nome do plano de saúde                                                                                       | 100            |
 | assistencia_saude_plano_titular                     | Não         | Numérico | Servidor titular ou dependente. [0: Titular, 1: Dependente]                                                  | 1              |
 | informatica_conhecimentos_gerais                    | Não         | Numérico | Conhecimentos gerais de informática, de acordo com a Tabela 34                                               | 1              |
 | informatica_conhecimentos_nivel                     | Não         | Numérico | Nível de conhecimento em informática, de acordo com a Tabela 35                                              | 1              |

\* Este campo é obrigatório apenas se o Ato Legal estiver presente.

\*\* Campo obrigatório apenas se o representante legal e o tipo de representatividade do servidor estiverem presentes.

\*\*\* Este campo torna-se obrigatório caso o campo representatividade_tipo contenha o valor 4 ou 5.

\*\*\*\* Este campo torna-se obrigatório caso o campo representatividade_tipo contenha o valor 5.

---

### Atributo(s) da(s) chave(s) de identificação para importação de dados

* **chaves dependente (ordem de precedência)**
    1. nome, nome_mae, data_nascimento
    2. cpf
    3. pasep_pis_nit

* **chave dependência**
    * dependencia_tipo_dependencia e uma chave do servidor

* **chaves servidor (ordem de precedência)**
    1. servidor_vinculado_nome, servidor_vinculado_nome_mae, servidor_vinculado_data_nascimento
    2. servidor_vinculado_cpf
    3. servidor_vinculado_pasep_pis_nit

* **chave representante legal**
    * representante_legal_cpf

* **chave ato legal**
    * dependencia_ato_legal_tipo_ato, dependencia_ato_legal_numero, dependencia_ato_legal_ano

### Observações sobre atributos não obrigatórios e o processo de importação

1. **RG**
    * O atributo rg não é obrigatório, mas caso seja informado, o sistema de importação verificará a presença e validará os atributos rg_uf_expedicao, rg_orgao_expedidor e rg_data_emissao.
    * Caso os atributos rg_uf_expedicao, rg_orgao_expedidor e rg_data_emissao não seja informados em sua totalidade, nenhum destes atributos serão importados, incluindo o próprio atributo rg.
