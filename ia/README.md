# IA - Motor de Planejamento fitAi

## Funcionalidades
- Geração automática de planos de dieta e treino
- Cálculo de TDEE e macros baseado em dados do usuário
- Periodização de treinos (4-6 semanas)
- Ajustes semanais automáticos baseados em progresso
- Recomendações personalizadas de nutrição e exercícios

## Modelos e Regras

### Cálculo de TDEE
```
BMR (Mifflin-St Jeor) = (10 × peso(kg)) + (6,25 × altura(cm)) - (5 × idade) + 5 (homem) ou -161 (mulher)
TDEE = BMR × fator_atividade (1,4-1,8)
```

### Macros Padrão
- Proteína: 1,8-2,2 g/kg
- Gordura: 0,8-1,0 g/kg
- Carboidratos: restante das calorias

### Periodização de Treino
- Fase 1 (Semanas 1-4): Base técnica, volume moderado
- Fase 2 (Semanas 5-8): Aumento de intensidade, técnicas avançadas
- Rotação de exercícios: 30-40% trocados a cada fase

### Ajustes Automáticos
- Semanal: ajuste de ±100-150 kcal baseado em progresso
- Mensal: rotação de exercícios e variação de volume

## Implementação

### Opção 1: Regras Baseadas (Rule-based)
- Sistema de regras predefinidas
- Fácil de implementar e debugar
- Menos flexível

### Opção 2: Modelos de IA (LLMs)
- OpenAI GPT-4/Gemini para geração de planos
- Mais flexível e personalizado
- Custo mais alto, latência maior

### Opção 3: Híbrido
- Regras baseadas para cálculos fundamentais
- LLM para personalização e explicações

## Prompts Base
```
System: "Você é nutricionista esportivo e personal trainer. Com base nos dados do usuário, gere plano de dieta e treino."

User Context: { dados do usuário }

Output: {
  "calories": number,
  "macros": { protein, carbs, fat },
  "meal_plan": [...],
  "workout_plan": [...],
  "recommendations": [...]
}
```

## Status
**Aguardando definição de abordagem pelo MVPBuilderAI**

## Próximos Passos
1. Definir abordagem (rule-based vs LLM vs híbrido)
2. Implementar cálculos básicos (TDEE, macros)
3. Criar sistema de regras para periodização
4. Integrar com backend API
5. Testar com dados reais