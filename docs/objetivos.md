# Objetivos

## Objetivo geral
Projetar e avaliar um conjunto de políticas robustas para reduzir, de forma mensurável, o risco de prompt injection em aplicações NL2SQL, com foco em impedir ações indevidas no banco de dados.

## Objetivos específicos
1. Elaborar um modelo de ameaça e uma taxonomia de ataques aplicáveis a aplicações NL2SQL.
2. Definir um Policy Pack implementável e reutilizável, composto por políticas e controles de segurança.
3. Implementar um pipeline de execução mediada, no qual a LLM produza uma intenção estruturada sujeita a validação e políticas antes da geração e execução do SQL.
4. Construir um benchmark com perguntas legítimas, ground truth e uma suíte adversarial de prompts maliciosos.
5. Medir risco e utilidade com métricas padronizadas, comparando configurações com diferentes níveis de proteção.
6. Consolidar recomendações práticas para aplicação dessas políticas em pequenas empresas, considerando trade-offs, custo e viabilidade de implantação.
