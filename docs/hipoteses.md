# Hipóteses

## H1
Um policy engine determinístico reduz significativamente a taxa de sucesso do atacante quando comparado a uma arquitetura em que a LLM gera SQL diretamente.

## H2
O uso de uma representação intermediária, como JSON ou AST, aliado a uma compilação controlada para SQL, reduz bypass estrutural com menor taxa de falso bloqueio do que abordagens baseadas apenas em filtros superficiais, como regex.

## H3
A aplicação de limites de execução, como timeout, limite de linhas e restrições de custo, reduz o risco de DoS lógico com impacto pequeno na utilidade da aplicação.

## H4
A imposição de filtros obrigatórios por papel e escopo reduz tentativas de exfiltração e acesso indevido a dados, mesmo diante de ataques adaptativos.

## Expectativa de validação
As hipóteses serão avaliadas por comparação experimental entre configurações progressivas de segurança, considerando métricas de risco, utilidade, operação e governança.
