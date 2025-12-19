# Projeto_Final_CyberSec_VNW---Pishing---
Projeto Final - VNW - CyberSec - Mai Wolf S/A

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/c0dfbf53-4519-4d87-8f32-67a1b201f116" />

## Avaliação de Risco e Simulação de Engenharia Social (Phishing)

**Cliente:** Mai Wolf S/A  
**Setor:** Redes Sociais  
**Elaborado por:** Maiara Viegas – Analista de Segurança  
**Data:** 30/11/2025  

---

## Sumário
- Sumário Executivo  
- Objetivo  
- Escopo  
- Metodologia  
- Diagnóstico e Evidências  
- Análise de Risco  
- Proposta Técnica (Plano de Ação 80/20)  
- Indicadores de Segurança  
- Conclusão  

---

## 1. Sumário Executivo

Este relatório apresenta os resultados de uma **simulação controlada de ataque de engenharia social do tipo phishing**, realizada com o objetivo de avaliar o **risco humano** na postura de segurança da Mai Wolf S/A.

A simulação demonstrou que ataques simples, com baixo custo técnico, são suficientes para obter credenciais quando não existem controles de conscientização e validação por parte do usuário. O vetor explorado não foi uma falha tecnológica, mas sim o comportamento humano, hoje um dos principais pontos de falha em ambientes digitais.

Com base no princípio **80/20**, o relatório propõe ações de alto impacto e baixo esforço, focadas em reduzir drasticamente a efetividade desse tipo de ataque sem necessidade de investimentos complexos em infraestrutura.

---

## 2. Objetivo

Avaliar a exposição da Mai Wolf S/A a ataques de phishing por meio de uma simulação educacional e propor controles preventivos e corretivos que reduzam o risco de comprometimento de credenciais e acessos indevidos.

---

## 3. Escopo

A simulação teve caráter educacional e analítico, sem impacto em usuários reais ou sistemas de produção.

### Inclui:
- Simulação de phishing em ambiente controlado  
- Análise do comportamento do usuário diante de uma página falsa  
- Identificação dos principais erros humanos exploráveis  
- Proposição de medidas preventivas priorizadas  

### Não inclui:
- Uso de credenciais reais  
- Envolvimento de usuários reais  
- Ataques em ambientes produtivos
------

## 4. Metodologia

A metodologia adotada seguiu quatro etapas:

1. **Construção do cenário:** Criação de uma página falsa com aparência semelhante a um site legítimo de login.
2. **Execução da simulação:** Interação de uma vítima simulada com o ambiente.  
3. **Coleta de evidências:** Observação do fluxo de acesso e da captura de dados.
4. **Análise de risco:** Avaliação do impacto potencial caso o ataque ocorresse em ambiente real.

A abordagem foi intencionalmente simples, refletindo a realidade da maioria dos ataques de phishing bem-sucedidos.

---

## 5. Diagnóstico e Evidências

A simulação evidenciou os seguintes pontos críticos:

- **Alta confiança no aspecto visual** da página  
- **Ausência de verificação da URL** antes da inserção de credenciais  
- **Falsa sensação de segurança** ao reconhecer a interface do serviço  

Esses fatores indicam que **o atacante não precisa explorar vulnerabilidades técnicas**, apenas reproduzir elementos visuais familiares ao usuário.

---

## 6. Análise de Risco

| Fator de Risco                     | Impacto | Probabilidade | Observação |
|----------------------------------|---------|---------------|------------|
| Comprometimento de credenciais   | Alto    | Alto          | Ataque simples e fácil de replicar |
| Acesso indevido a contas         | Alto    | Médio         | Depende do nível de privilégio |
| Escalada para outros sistemas    | Alto    | Médio         | Uso de credenciais reutilizadas |
| Impacto reputacional             | Médio   | Médio         | Vazamento ou uso indevido de contas |

**Conclusão do risco:**  
O phishing representa um **risco crítico**, principalmente em ambientes que dependem fortemente de redes sociais e identidade digital.

---

## 7. Proposta Técnica – Plano de Ação (80/20)

### 7.1 Quick Wins – 30 dias

**Ação 1 – Conscientização objetiva sobre phishing**  
Treinamento curto e prático, com exemplos reais de páginas falsas e URLs maliciosas.

**Ação 2 – Implementação obrigatória de MFA**  
Reduz drasticamente o impacto do comprometimento de senha.

**Ação 3 – Política de verificação de links**  
Orientação clara: nenhum login deve ser realizado a partir de links recebidos por mensagens ou e-mails.

**Ação 4 – Uso de gerenciadores de senha**  
Gerenciadores só preenchem credenciais em domínios legítimos, bloqueando phishing visual.

---

### 7.2 Controles Complementares (médio prazo)

- Simulações periódicas de phishing educacional  
- Canal simples para reporte de links suspeitos  
- Inclusão do risco humano no programa de segurança  

---

## 8. Indicadores de Segurança (KPIs)

- Taxa de usuários que identificam phishing em simulações  
- Redução de cliques em links suspeitos  
- Percentual de contas com MFA habilitado  
- Tempo médio de resposta a incidentes reportados  

Esses indicadores permitem medir a **maturidade do comportamento humano** ao longo do tempo.

---

## 9. Conclusão

A simulação confirmou que **o fator humano continua sendo um dos maiores vetores de ataque**, mesmo em cenários com tecnologias adequadas.

Pequenas ações, bem direcionadas, têm potencial de **reduzir significativamente o risco**, sem demandar investimentos elevados.

Ao tratar engenharia social como um risco estratégico, e não apenas educacional, a Mai Wolf S/A fortalece sua postura de segurança e reduz a probabilidade de incidentes com impacto operacional e reputacional.



