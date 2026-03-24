# Especificação do Banco de Dados

## Entidades Principais

### User (Usuário)
- `id`: UUID (PK)
- `username`: String (Unique)
- `email`: String (Unique)
- `role`: Enum (Admin, Teacher, Student)
- `date_joined`: DateTime

### Course (Curso)
- `id`: UUID (PK)
- `title`: String
- `slug`: String
- `description`: Text
- `instructor_id`: FK(User)
- `status`: Enum (Draft, Published)

### Module (Módulo)
- `id`: UUID (PK)
- `course_id`: FK(Course)
- `title`: String
- `order`: Integer

### Lesson (Aula/Conteúdo)
- `id`: UUID (PK)
- `module_id`: FK(Module)
- `title`: String
- `content_type`: Enum (Video, PDF, Text)
- `file_url`: String
- `text_body`: Text
