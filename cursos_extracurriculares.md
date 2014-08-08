# Layout de exportação dos dados de cursos extracurriculares do servidor para o GestPrev Next

### Tabela de atributos

 | Atributo                         | Obrigatório | Tipo     | Descrição                                                                 | Tamanho máximo |
 | :------------------------------- | :---------- | :------- | :------------------------------------------------------------------------ | -------------: |
 | curso_ec_nome                    | Não         | Caracter | Nome do cursos extracurricular                                            | 100            |
 | curso_ec_carga_horaria           | Não         | Numérico | Carga horária do curso extra (em horas)                                   | -              |
 | curso_ec_data_inicio             | Não         | Data     | Data de início do curso extracurricular, preencher no formato DD/MM/AAAA  | 10             |
 | curso_ec_data_termino            | Não         | Data     | Data de término do curso extracurricular, preencher no formato DD/MM/AAAA | 10             |
 | curso_ec_nome_instituicao        | Não         | Caracter | Nome da instituição que realizou o curso extracurricular                  | 100            |
 | servidor_vinculado_nome          | Sim         | Caracter | Nome completo do servidor vinculado                                       | 80             |
