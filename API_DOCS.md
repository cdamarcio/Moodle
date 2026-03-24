Documentação da API (Endpoints)

A API segue os princípios REST e utiliza JSON para comunicação.

1. Autenticação

Método

Endpoint

Descrição

POST

/api/auth/register/

Registo de novo utilizador.

POST

/api/auth/login/

Login e obtenção de Token JWT.

2. Cursos

Método

Endpoint

Descrição

GET

/api/courses/

Listagem de todos os cursos publicados.

POST

/api/courses/

Criação de novo curso (Apenas Professores).

GET

/api/courses/{id}/

Detalhes de um curso específico.

PUT

/api/courses/{id}/

Atualização de curso.

3. Conteúdo (Aulas)

Método

Endpoint

Descrição

GET

/api/courses/{id}/modules/

Listagem de módulos e lições do curso.

POST

/api/lessons/{id}/complete/

Marcar lição como concluída.

4. Matrículas e Progresso

Método

Endpoint

Descrição

POST

/api/enrollments/

Matricular aluno num curso.

GET

/api/users/me/progress/

Obter progresso do aluno logado.
