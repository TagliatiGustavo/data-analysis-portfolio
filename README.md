# Portfólio de Análise de Dados: Operação de Equipes Volantes

## Objetivo
Analisar os dados de visitas de equipes volantes aos prédios, considerando a periodicidade das visitas e a distribuição das equipes nos estados de Minas Gerais, Rio de Janeiro, São Paulo e Espírito Santo. Utilizei SQL e Excel para conduzir a análise e gerar insights valiosos para otimização de recursos e melhoria na tomada de decisão.

## 1. Distribuição de Visitas por Periodicidade em Cada Estado

**Objetivo:**
Entender como as visitas são distribuídas ao longo das diferentes periodicidades (diária, semanal, quinzenal, mensal e trimestral) em cada estado.

**SQL Query:**
```sql
SELECT estado, periodicidade, COUNT(*) AS total_visitas
FROM visitas
GROUP BY estado, periodicidade;
