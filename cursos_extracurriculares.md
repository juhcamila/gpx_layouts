# Layout de exportação dos dados de cursos extracurriculares do servidor para o GestPrev Next

### Tabela de atributos

 | Atributo                           | Obrigatório | Tipo     | Descrição                                                                  | Tamanho máximo |
 | :-------------------------------   | :---------- | :------- | :------------------------------------------------------------------------  | -------------: |
 | curso_ec_nome                      | Sim         | Caracter | Nome do cursos extracurricular                                             | 100            |
 | curso_ec_carga_horaria             | Sim         | Numérico | Carga horária do curso extra (em horas)                                    | -              |
 | curso_ec_data_inicio               | Sim         | Data     | Data de início do curso extracurricular, preencher no formato DD/MM/AAAA   | 10             |
 | curso_ec_data_termino              | Sim         | Data     | Data de término do curso extracurricular, preencher no formato DD/MM/AAAA  | 10             |
 | curso_ec_nome_instituicao          | Sim         | Caracter | Nome da instituição que realizou o curso extracurricular                   | 100            |
 | pessoa_vinculada_nome\*            | Sim         | Caracter | Nome completo da pessoa vinculado                                          | 80             |
 | pessoa_vinculada_nome_mae\*        | Não         | Caracter | Nome completo da mãe da pessoa vinculado                                   | 80             |
 | pessoa_vinculada_data_nascimento\* | Não         | Data     | Data de nascimento da pessoa vinculado , preencher no formato DD/MM/AAAA   | 10             |
 | pessoa_vinculada_cpf\*             | Não         | Caracter | CPF, preencher somente com números da pessoa vinculado                     | 11             |
 | pessoa_vinculada_pasep_pis_nit\*   | Não         | Caracter | Número de PIS/PASEP/NIT da pessoa vinculado, preencher somente com números | 11             |

\* Pessoa pode ser: Servidor, Dependente ou Pensionista

---

### Atributo(s) da chave de identificação para importação de dados

* **chave curso extracurricular**
    * curso_ec_nome, curso_ec_carga_horaria, curso_ec_data_inicio, curso_ec_data_termino, curso_ec_nome_instituicao e uma chave de pessoa
    * ** chaves de pessoa **
        1. pessoa_vinculada_nome, pessoa_vinculada_nome_mae, pessoa_vinculada_data_nascimento
        2. pessoa_vinculada_cpf
        3. pessoa_vinculada_pasep_pis_nit
