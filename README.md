# API To-Do List

## Descrição do Projeto
API RESTful simples para gerenciamento de tarefas (To-Do List), desenvolvida com Node.js e Express.  
Permite criar, listar, atualizar e remover tarefas, armazenando informações como título, descrição e status.

**Tecnologias utilizadas:**
- Node.js 22
- Express
- Jest e Supertest para testes automatizados
- GitHub Actions para Integração Contínua (CI)
- UUID para identificação única das tarefas

---

## Instruções de Instalação e Execução

1. Clone o repositório:
```bash
git clone <URL_DO_REPOSITORIO_DA_LARISSA>
Entre na pasta do projeto:

bash
Copiar código
cd todo-api
Instale as dependências:

bash
Copiar código
npm install
Rodar a API em modo desenvolvimento:

bash
Copiar código
npm run dev
Rodar a API normalmente:

bash
Copiar código
npm start
Rodar os testes automatizados:

bash
Copiar código
npm test
Documentação da API
Método	Rota	Descrição	Corpo (JSON)
POST	/tasks	Criar nova tarefa	{ "title": "Comprar leite", "description": "Ir ao supermercado" }
GET	/tasks	Listar todas as tarefas	-
GET	/tasks/:id	Consultar tarefa específica	-
PUT	/tasks/:id	Atualizar título, descrição ou status	{ "title": "Novo título", "status": "concluida" }
DELETE	/tasks/:id	Remover tarefa pelo ID	-

Integração Contínua (CI)
A CI foi configurada usando GitHub Actions para:

Rodar automaticamente os testes a cada push ou pull request no branch principal.

Garantir que o código permaneça funcional e testado antes de qualquer merge.

Arquivo do workflow: .github/workflows/ci.yml

Testes de Software
Automatizados: 5 testes Jest/Supertest cobrindo:

Criação de tarefa

Rejeição de título vazio

Listagem de tarefas

Atualização de tarefa

Exclusão de tarefa

Manuais: (exemplo de tabela para entregar)

Cenário	Passos	Entrada	Resultado Esperado
Criar tarefa	POST /tasks	{ "title": "Comprar leite" }	Tarefa criada com status "pendente"
Criar tarefa sem título	POST /tasks	{ "title": "" }	Retorno de erro
Listar todas as tarefas	GET /tasks	-	Lista contendo todas as tarefas
Atualizar tarefa	PUT /tasks/:id	{ "status": "concluida" }	Tarefa atualizada
Deletar tarefa	DELETE /tasks/:id	-	Tarefa removida

Componente Extensionista
Integração Contínua (CI):
Permite que estudantes iniciantes aprendam boas práticas de desenvolvimento, garantindo que alterações não quebrem o sistema e promovendo hábitos profissionais de qualidade.

Usos possíveis da API:
Aplicações cotidianas: lista de tarefas pessoais, lembretes, gerenciamento de atividades de equipes.
Projetos sociais: controle de tarefas em voluntariados, monitoramento de serviços comunitários ou educacionais.

Testes de software:
Aumentam confiança, qualidade e segurança do sistema, essencial para sistemas de serviços públicos, educação e saúde, garantindo que erros não impactem os usuários finais.

Autor
LarissaBarbosadaSilva
