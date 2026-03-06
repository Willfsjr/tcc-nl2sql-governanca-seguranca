# Problema de Pesquisa

## Contexto
A adoção de aplicações baseadas em modelos de linguagem para consulta de bancos de dados por linguagem natural tem ampliado o acesso à informação por usuários não especializados em SQL. No entanto, essa mesma facilidade amplia a superfície de risco, pois a entrada em linguagem natural pode ser manipulada por meio de prompt injection para induzir o sistema a executar ações indevidas, contornar escopos obrigatórios, acessar dados sensíveis ou gerar consultas abusivas.

## Problema central
Em aplicações NL2SQL, como reduzir o risco de prompt injection e de ações indevidas no banco de dados sem comprometer excessivamente a utilidade, a auditabilidade e a experiência de uso do sistema?

## Questões específicas
- Como impedir que prompts maliciosos levem à geração de comandos indevidos?
- Como garantir que consultas permaneçam dentro do escopo permitido por papel, empresa, filial, período ou tenant?
- Como reduzir riscos de exfiltração de dados e de consultas abusivas sem gerar bloqueios excessivos?
- Como estruturar políticas reutilizáveis para diferentes implementações NL2SQL?
- Como medir, de forma objetiva, a redução de risco e o impacto na utilidade?

## Justificativa do problema
O avanço do uso de IA aplicada a dados torna relevante a construção de mecanismos de governança, controle e auditoria que permitam o uso seguro dessas aplicações em contextos organizacionais reais. Em pequenas e médias empresas, especialmente, soluções reutilizáveis e de implantação viável podem apoiar o uso responsável de consultas em linguagem natural sem exigir arquiteturas excessivamente complexas.
