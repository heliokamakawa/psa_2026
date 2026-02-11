# Análise da qualidade do software visando confiabilidade 

### Autores: Ali Osmar ; Ariel Machado; Gustavo Marangoni, Rômulo Bogoni.
Profº Dr. Hélio Kamaka

### 1. Escopo
Aplicação da Inteligência Artificial na Automação e Otimização do Desenvolvimento de Software

### 2.Introdução, justificativa e conexão
Este projeto tem como objetivo avaliar o uso de múltiplas Inteligências Artificiais como agentes de apoio à análise, refatoração e melhoria da qualidade de código de um projeto existente denominado Apollo. A proposta parte do princípio de que diferentes modelos de IA possuem abordagens distintas de raciocínio, leitura de código e aplicação de padrões, o que pode gerar resultados variados em termos de qualidade, legibilidade, arquitetura e manutenção.

Ao comparar essas abordagens, buscamos entender quais ganhos reais a IA pode trazer para o processo de engenharia de software, indo além de simples correções sintáticas e focando em qualidade estrutural e boas práticas.
### 3. Objetivo Geral
Utilizar três IAs distintas para:
- Analisar códigos do projeto Apollo
- Refatorar os trechos analisados
- Aplicar padrões de qualidade previamente definidos
- Comparar os resultados gerados por cada IA
- Avaliar diferenças técnicas, conceituais e arquiteturais
### 4. Estratégia Geral
Serão selecionadas três IAs diferentes, tratadas como agentes independentes. Nenhuma IA terá acesso às respostas das outras. Cada IA receberá:
O mesmo trecho de código do projeto da Apollo
O mesmo prompt padrão
As mesmas regras de qualidade
Isso garante isonomia no experimento.
### 5. Objetivos Específicos 
O prompt será o principal instrumento de controle de qualidade. Ele deverá: Posicionar a IA como engenheira de software

Você é um engenheiro de software sênior especializado em análise de qualidade e confiabilidade de código. Sua tarefa é realizar uma avaliação abrangente da confiabilidade do código-fonte fornecido.

### Contexto do Projeto
[Descrever brevemente o projeto, linguagem(s) de programação, frameworks utilizados e domínio de aplicação]

### Objetivos da Análise
Avaliar a confiabilidade do código considerando os seguintes aspectos críticos:

1. Tratamento de Erros e Exceções
- Identificar pontos de falha potenciais sem tratamento adequado
- Avaliar a robustez dos mecanismos de try-catch/error handling
- Verificar validação de inputs e saídas
- Analisar estratégias de recuperação de falhas

2. Qualidade e Manutenibilidade
- Complexidade ciclomática e cognitive complexity
- Duplicação de código e violações do princípio DRY
- Aderência a padrões de design e boas práticas
- Legibilidade e clareza do código

3. Gestão de Recursos
- Gerenciamento adequado de memória e recursos (conexões, arquivos, streams)
- Prevenção de memory leaks e resource leaks
- Uso apropriado de garbage collection ou gerenciamento manual

4. Segurança
- Vulnerabilidades conhecidas (SQL injection, XSS, CSRF, etc.)
- Validação e sanitização de dados
- Gestão segura de credenciais e informações sensíveis
- Implementação de controles de autenticação e autorização

5. Concorrência e Thread-Safety
- Condições de corrida (race conditions)
- Deadlocks potenciais
- Sincronização adequada de recursos compartilhados
- Uso correto de primitivas de concorrência

6. Testes e Cobertura
- Cobertura de testes unitários, integração e end-to-end
- Qualidade e efetividade dos testes
- Casos edge e cenários de falha cobertos

7. Logging e Monitoramento
- Adequação dos logs para debugging e auditoria
- Estratégias de monitoramento de saúde da aplicação
- Rastreabilidade de erros e exceções

## Formato de Entrega
Para cada categoria avaliada, forneça:
1. **Pontuação de Confiabilidade** (1-10, onde 10 é excelente)
2. **Principais Problemas Identificados** com exemplos específicos do código
3. **Severidade** (Crítica, Alta, Média, Baixa)
4. **Recomendações Práticas** para correção
5. **Prioridade de Implementação**

## Resultado Final
- **Score Geral de Confiabilidade** (média ponderada)
- **Resumo Executivo** com os 5 riscos mais críticos
- **Roadmap de Melhorias** priorizando ações de maior impacto
- **Métricas de Acompanhamento** sugeridas

## Instruções Adicionais
- Seja específico ao citar problemas, incluindo nomes de arquivos e linhas quando possível
- Forneça exemplos de código corrigido quando apropriado
- Considere o contexto e requisitos do projeto ao fazer recomendações
- Priorize problemas que impactem diretamente usuários finais ou integridade dos dados.

### 6. Tecnologias e Ferramentas Utilizadas
Escolhemos reaproveitar um projeto que foi desenvolvido por nós, no 3° ano do curso de engenharia de software nas matérias de Projeto integrador e Construção de Software, foi retirado uma parte do código para fazer a análise. Utilizamos 3 IA’s distinas: chat GPT ; Cloude ;

### 7. Descrição da Prática
...

### 8. Cronograma das Atividades Práticas
...

### 9. Materiais de Estudo 
https://www.researchgate.net/profile/Daniel-Ajiga/publication/383410449_Enhancing_software_development_practices_with_AI_insights_in_high-_tech_companies/links/66cb63b4920e05672e50416d/Enhancing-software-development-practices-with-AI-insights-in-high-tech-companies.pdf

https://www.researchgate.net/profile/Gregory-Talavera/publication/388835184_AI-Driven_Developer_Performance_Metrics_Enhancing_Agile_Software_Development/links/67a90c8d8311ce680c5acb7b/AI-Driven-Developer-Performance-Metrics-Enhancing-Agile-Software-Development.pdf

https://pdf.sciencedirectassets.com/271670/1-s2.0-S0378720625X00100/1-s2.0-S0378720626000066/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEOn%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIQC17GqmmEDi98xN5grAcwNO46ygxfUfOaX7sP4DHeMqcQIgJ1ULBciq8vrqLMI6HbDLrpCV6YBZNWDJQZxPeCBO5tIqvAUIsf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAFGgwwNTkwMDM1NDY4NjUiDDG6WAfzXOYYKd40EyqQBVN0kLBzrp3umiWEWBYTDO0LogWhcpivgZa%2BX23Kgl5hmUCCtckae%2BlRjFfBNWymRQCYLVymteIX2Pl9OsBEAZG6sI3uKte8G%2BCKetue%2FGCjSuziyJDPUJjdGD6LeA%2FL5Eqs%2FHAJi7iyeWGirjIltTq9a9BYroiqD3r0sPsL1lvRemo0agVAfhynURAqaZ%2BikfCBuzFrmsw37YpxIyxmDP8B0VaKq2GpIiCo0lGhOVPRRQhrSx9CR1ILumNhJBPcP3U6N8Koe0buuCdK4OkkuNCAjLoSnlo%2BasmFWFd29CG52%2BrUJfrdZ66wj0YDN6tjAKCTy98LQS0igTz9i3DhFSDhtEBJa%2BX3Brqdj%2B8CHhaCcjLmSpwCJ1FJFHACCKWj36AK0eemiO32FKQkCuFJMI%2BmTLATq43kZPXSvF%2FK3VjRZyMlGhe4%2FwjnDM9eF3Tm8CXU%2F%2Bp6CzhWavsGvfLnheGvRgB5pRtmcqIQXMpypSWTkmjMxHwtvzFaWCwQJR%2FcdaUeHtd301ucD7TNV8TEmwNzeyrfttA%2FNmwRjmWHbckCw5lVSAtXbjDj3ARBiKcuy7Du%2FIUot1O6f%2BVzykgSJFn0rwQb%2BGEQrH3LcfiGolmHVPY8iVAAe9rt9IOk0pCJ%2FO6MpSEzyflDMOFvi38E9dthl2uS5DHjm4Y7a5OY6abbNtucClhjQNGjWzj6CzaQNzQpV09Bf%2BV1NDpjXdudBwDQJvkOT9cSlCoM4s6Ef5lh%2BzkD67GGNUwINLeUy0c9roSkggxkUNKIpOOzjN4uNyUYdR%2B06c6e6JAfQWYzZ10WeKvOT67nx67HUvx7iPT%2B%2B0CDnpVDuofN4v2uKM4Ia2%2BiyPhk9QRkYxfBRw%2B2x%2FZWMMGSr8wGOrEBa0ks0U5xxFB2HwBrjLj%2F6b7hGHznlpSAavvfW9GGl2bXKnVutMKPUX4U%2Fw6JeblbwXOqkU1%2FvlAvZqp50YxU9lYlnQCHOEPDwkGJF7tTM5oWWpCRg08oqCjH4ehd2m3ly3DVr0Wj7QcpageCrCnE%2BkK9sksH%2BExyQKRg2vGItpng7NS1ia16oAQ5wc2ssEAzuqiCi4rJnKygw6wlVDd6Mt7EERNi%2FF4dTONOcmPqyMLg&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20260211T005705Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY6L3QSJN7%2F20260211%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=c66acfc3c0f93bbf9ad7fce4044af89c0b396774966f729b92f4682255cd6ddd&hash=affa1e8e294a2f90705591dd79a65e120fa58645d66ccd91715835039e104e6d&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0378720626000066&tid=spdf-bc9f24b4-106b-418e-9195-5d5103053c4f&sid=d31580818c82d24c310b53e7d7c479715288gxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&rh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=061557050005045d07&rr=9cbfe3dd480a0343&cc=br

https://www.researchgate.net/profile/Nathalia-Nascimento-4/publication/370938349_Comparing_Software_Developers_with_ChatGPT_An_Empirical_Investigation/links/6508f70e82f01628f030a202/Comparing-Software-Developers-with-ChatGPT-An-Empirical-Investigation.pdf

https://ietresearch.onlinelibrary.wiley.com/doi/pdf/10.1049/iet-sen.2016.0095

