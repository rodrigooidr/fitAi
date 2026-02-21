# Testes Automatizados - fitAi

## Estratégia de Testes
- **Testes Unitários:** Componentes individuais, funções utilitárias
- **Testes de Integração:** APIs, serviços, banco de dados
- **Testes End-to-End (E2E):** Fluxos completos do usuário
- **Testes de IA:** Validação de cálculos e regras de negócio

## Tecnologias de Teste

### Frontend (React Native)
- Jest + React Testing Library
- Detox para testes E2E
- Mock de APIs e serviços

### Backend (Node.js)
- Jest ou Mocha + Chai
- Supertest para testes de API
- Mock de banco de dados (ou SQLite em memória)

### IA/Regras de Negócio
- Testes unitários para funções de cálculo
- Testes de validação para prompts e respostas de IA
- Testes de regras de periodização e ajustes

## Cobertura de Testes Alvo
- **Mínimo:** 80% cobertura de código
- **Crítico:** 100% cobertura para cálculos de saúde e segurança
- **E2E:** Fluxos principais (onboarding, log de treino, ajustes)

## Testes Críticos a Implementar

### Cálculos de Saúde
- TDEE calculation (várias fórmulas)
- Macros calculation (limites seguros)
- Progressão de carga (segurança)
- Ajustes calóricos (limites)

### Fluxos de Usuário
- Onboarding completo
- Geração de plano
- Log de treino e refeição
- Ajustes automáticos
- Exportação de PDF

### Segurança
- Autenticação/autorização
- Validação de dados sensíveis
- Proteção contra dados inválidos

## Status
**Aguardando implementação pelo QualityAssuranceAI**

## Próximos Passos
1. Configurar ambiente de testes
2. Implementar testes unitários básicos
3. Criar testes de integração para APIs
4. Implementar testes E2E para fluxos principais
5. Configurar CI para execução automática de testes