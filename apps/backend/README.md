# Backend API - fitAi

## Tecnologia
**Node.js** com **Express/Fastify** + **PostgreSQL** (Supabase) ou **Firebase**

## Principais Funcionalidades
- Autenticação de usuários (JWT, OAuth)
- Gerenciamento de perfis e dados de saúde
- Motor de IA para geração de planos (dieta + treino)
- API para logs de treino e nutrição
- Cálculo de progresso e ajustes automáticos
- Geração de PDFs (planos e relatórios)
- Sistema de notificações

## Endpoints Principais (planejados)
```
POST   /auth/register      # Registro de usuário
POST   /auth/login         # Login
POST   /auth/forgot        # Recuperação de senha

GET    /me                 # Perfil do usuário
PUT    /me                 # Atualizar perfil

POST   /plans/generate     # Gerar plano (chama IA)
GET    /plans/current      # Plano atual

POST   /workouts/log       # Log de treino
POST   /meals/log          # Log de refeição

GET    /progress           # Dados de progresso
GET    /export/plan.pdf    # Exportar plano em PDF

POST   /automations/schedule # Agendar ajustes automáticos
```

## Banco de Dados
Modelo relacional com tabelas:
- `users` (usuários)
- `profiles` (dados de saúde)
- `measurements` (medições)
- `plans` (planos de dieta/treino)
- `workout_logs` (logs de treino)
- `diet_logs` (logs de alimentação)

## Status
**Aguardando definição de stack tecnológica pelo MVPBuilderAI**

## Próximos Passos
1. Definir stack (Node.js + PostgreSQL vs Firebase)
2. Configurar banco de dados
3. Criar estrutura básica da API
4. Implementar autenticação
5. Integrar com serviço de IA