# fitAi - Fitness AI Assistant

## Visão do Projeto
App de saúde/fitness que coleta dados físicos e objetivos do usuário, gera automaticamente dieta e treino com IA, acompanha progresso, periodiza o treino, ajusta macros e oferece vídeos de execução.

## Fábrica de Software com Agentes
Este projeto está sendo desenvolvido por uma **fábrica de software automatizada com agentes de IA** que executam cada etapa do ciclo de desenvolvimento:

### Agentes Especializados
1. **ValidatorAI** - Valida requisitos e questiona ambiguidades
2. **MVPBuilderAI** - Cria estrutura do projeto e define stack tecnológica
3. **CoreDevAI** - Implementa features com code review automatizado
4. **QualityAssuranceAI** - Executa testes automatizados e valida qualidade
5. **DeploymentAI** - Gerencia CI/CD e releases automatizados
6. **Clawdio (Orquestrador)** - Coordena todos os agentes e monitora progresso

### Dashboard de Monitoramento
- **Dashboard Público:** https://rodrigooidr.github.io/fitAi/
- **Status em Tempo Real:** Acompanhamento das atividades de cada agente
- **Logs de Atividades:** Histórico completo de todas as ações automatizadas

## Arquitetura MVP

### Frontend
- **Tecnologia:** React Native (Expo) para iOS/Android
- **Principais Telas:** Onboarding, Home (Hoje), Treino, Nutrição, Progresso, Configurações
- **Estado:** Redux Toolkit ou Context API
- **Estilização:** Tailwind CSS (NativeWind) ou Styled Components

### Backend
- **Tecnologia:** Node.js com Express ou Fastify
- **Banco de Dados:** PostgreSQL (Supabase) ou Firebase
- **Autenticação:** JWT + OAuth (Google/Apple)
- **IA:** OpenAI API (GPT-4) ou Gemini para geração de planos

### IA/ML
- **Motor de Planejamento:** Regras baseadas em TDEE + macros + periodização
- **Ajustes Automáticos:** Algoritmos de ajuste semanal baseados em progresso
- **Recomendações Personalizadas:** Sistema de recomendação baseado em histórico

### Infraestrutura
- **CI/CD:** GitHub Actions
- **Deploy:** Vercel (frontend) + Railway/Render (backend)
- **Monitoramento:** Sentry + LogRocket
- **Notificações:** OneSignal ou Expo Notifications

## Estrutura de Diretórios
```
fitAi/
├── apps/
│   ├── frontend/     # React Native app
│   └── backend/      # Node.js API
├── ia/               # IA models, prompts, rules
├── tests/            # Testes automatizados
├── docs/             # Documentação e dashboard
├── artifacts/        # Artefatos de validação
└── .github/          # CI/CD workflows
```

## Status Atual
✅ **Fase 1 - Definição:** Concluída  
✅ **Fase 2 - Validação:** Concluída (artefatos gerados)  
🔄 **Fase 3 - MVP Skeleton:** Em andamento  
⬜ **Fase 4 - Desenvolvimento:** Pendente  
⬜ **Fase 5 - Testes:** Pendente  
⬜ **Fase 6 - Deploy:** Pendente  

## Como Contribuir
Este projeto está sendo desenvolvido automaticamente por agentes de IA. Para contribuir manualmente:

1. Fork o repositório
2. Crie uma branch para sua feature
3. Envie um Pull Request

## Licença
MIT