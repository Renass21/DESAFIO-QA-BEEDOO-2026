# DESAFIO-QA-BEEDOO-2026

**Qual você acredita ser o objetivo da aplicação?**

O objetivo da aplicação é servir como um Painel Administrativo (CMS) para o gerenciamento de cursos. O sistema deve permitir o ciclo completo de um CRUD (Create, Read, Update, Delete), possibilitando o controle de vagas, períodos, instrutores, descrições detalhadas e o direcionamento externo via URL.

**Quais são os principais fluxos disponíveis?**

Atualmente, os fluxos funcionais identificados são a Criação (Cadastrar) e a Visualização (Listar) dos cursos.
(Nota: Identifiquei que os fluxos de Edição e Exclusão, embora esperados, apresentam falhas críticas ou ausência de implementação funcional).

**Quais pontos do sistema você considera mais críticos para teste?**

Por se tratar de um painel administrativo, os pontos de maior risco são:

- Segurança e Autenticação: A ausência de controle de acesso permite que usuários anônimos manipulem dados sensíveis.
- Integridade de Dados (Formulários): A falta de validações (sanitização de inputs e limites de caracteres/datas) compromete a persistência correta das informações e a estabilidade do banco de dados.
- Persistência da URL: Funcionalidade vital para o redirecionamento do aluno ao curso, que atualmente apresenta falha de salvamento.

**
Utilizei a técnica de Testes Exploratórios para mapear as funcionalidades existentes e identifiquei inconsistências críticas em relação às boas práticas de CRUD e segurança. Documentei os Casos de Teste baseados nos requisitos ideais e os bugs encontrados conforme o comportamento atual da aplicação.

Observações de Evidências e Bug Reports:
 
https://docs.google.com/spreadsheets/d/1E3-xrsVUrXJjLGruWErOPlCMasKL9p2xDKeDdVuVgvM/edit?usp=sharing