# Regras de Negócio e Fluxos

## 1. Regras de Negócio (RN)
* **RN01 (Acesso):** Um aluno só visualiza o conteúdo de um curso se estiver com a matrícula ativa.
* **RN02 (Certificação):** O certificado só é liberado se o aluno atingir 100% de visualização das aulas e 70% de acerto nos testes.
* **RN03 (Edição):** O professor só pode editar cursos que ele mesmo criou ou que lhe foram atribuídos pelo Admin.

## 2. Casos de Uso Principais
### UC01: Realizar Matrícula
1. Aluno navega pelo catálogo.
2. Aluno seleciona o curso desejado.
3. Aluno clica em "Inscrever-se".
4. O sistema valida os pré-requisitos e libera o acesso ao Módulo 1.

### UC02: Adicionar Conteúdo
1. Professor acessa o painel de instrutor.
2. Seleciona o curso e o módulo.
3. Faz upload do PDF ou cola o link do vídeo.
4. O sistema processa o arquivo e atualiza a grade para os alunos.
