# TCC - NL2SQL, Governança e Segurança

Este repositório reúne a estrutura, os estudos e a evolução do meu Trabalho de Conclusão de Curso em Ciência da Computação.

## Tema
Políticas robustas e avaliação de risco para aplicações com LLMs integradas a SQL, com foco em mitigação de prompt injection e prevenção de ações indevidas.

## Contexto
Sistemas NL2SQL permitem consultar bancos relacionais por meio de linguagem natural. Apesar do ganho de usabilidade, esse modelo traz riscos relevantes quando a aplicação depende de uma LLM para interpretar solicitações e transformá-las em consultas ao banco.

O foco deste trabalho não é “criar uma LLM segura”, mas definir e avaliar um conjunto de políticas e controles reutilizáveis que reduzam o risco de forma mensurável em implementações NL2SQL.

## Objetivo geral
Projetar e avaliar um conjunto de políticas robustas para reduzir, de forma mensurável, o risco de prompt injection em aplicações NL2SQL, com foco em impedir ações indevidas no banco de dados.

## Objetivos específicos
- elaborar modelo de ameaça e taxonomia de ataques aplicáveis a NL2SQL
- definir um Policy Pack implementável e reutilizável
- implementar um pipeline de execução mediada
- construir benchmark com perguntas legítimas e suíte adversarial
- medir risco e utilidade com métricas padronizadas
- consolidar recomendações práticas para pequenas empresas

## Escopo
- entrada: pergunta do usuário em linguagem natural
- saída: consulta somente leitura e resposta analítica
- bancos relacionais: Oracle e PostgreSQL
- sem leitura de documentos externos
- sem automações externas
- foco em prevenção de ações indevidas

## Estrutura do repositório
- `docs/` → tema, problema, objetivos, justificativa e capítulos
- `referencias/` → bibliografia e materiais de apoio
- `notas/` → anotações de estudo
- `prototipo/` → implementação experimental
- `resultados/` → tabelas, gráficos e análises

## Pergunta central
Como reduzir o risco de prompt injection em aplicações NL2SQL sem comprometer excessivamente a utilidade, a auditabilidade e a experiência de uso?

## Hipóteses
- um policy engine determinístico reduz a taxa de sucesso do atacante
- uma representação intermediária com compilação controlada reduz bypass estrutural
- limites de execução reduzem DoS lógico com pequeno impacto na utilidade
- filtros obrigatórios por papel e escopo reduzem exfiltração de dados

## Status
Em desenvolvimento.

## Autor
Willian Ferreira
