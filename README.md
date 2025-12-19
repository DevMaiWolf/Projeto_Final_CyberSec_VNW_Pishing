# Projeto_Final_CyberSec_VNW---Pishing---
Projeto Final - VNW - CyberSec - Mai Wolf S/A

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/c0dfbf53-4519-4d87-8f32-67a1b201f116" />

## Avaliação de Risco e Simulação de Engenharia Social (Phishing)

**Cliente:** Mai Wolf S/A  
**Setor:** Redes Sociais  
**Elaborado por:** Maiara Viegas – Analista de Segurança  
**Data:** 30/11/2025  

---

## 1. Sumário Executivo

Este relatório detalha a simulação de um ataque de **Phishing de Credenciais**. O teste validou que a semelhança visual de páginas fraudulentas induz usuários à exposição de dados sensíveis. Para mitigar esse risco de forma escalável, esta proposta integra automação via Python para detecção precoce e uma arquitetura de **Defesa em Profundidade**, alinhada às melhores práticas de **Blue Team**.

---

## 2. Objetivo

Avaliar a vulnerabilidade do fator humano e implementar mecanismos automatizados de resposta para garantir que credenciais capturadas não comprometam a integridade da infraestrutura da **Mai Wolf S/A**.

---

## 3. Metodologia e Escopo

- **Ambiente Controlado:** Criação de página fictícia para captura de credenciais de teste.
- **Simulação:** Demonstração da interação da vítima com o site falso e observação de falhas na validação da URL.
- **Automação:** Desenvolvimento de scripts em Python para monitoramento de logs de acesso e identificação de anomalias.

---

## 4. Análise de Risco Humano e Diagnóstico

A simulação revelou que o maior ponto fraco é o comportamento do usuário diante de interfaces familiares.

- **Confiança Visual:** A réplica visual anulou a cautela técnica.
- **Ausência de Verificação:** Falta de hábito em auditar a URL antes da inserção de dados.
- **Ponto Único de Falha:** Dependência exclusiva de senha para acesso aos sistemas.

---

## 5. Proposta Técnica: Automação e Resposta (80/20)

Para elevar a postura de segurança, propõe-se a integração de ferramentas gerenciáveis pelo time de SRE.
log_analize.py
<img width="1142" height="514" alt="image" src="https://github.com/user-attachments/assets/5a5b8fb1-40de-40a1-aeff-80cfecb09803" />

### 5.1. Implementação de "Scripts de Defesa" (Python)

Para reduzir a dependência da atenção do usuário, serão utilizados scripts para:

- **Monitoramento de Domínios:** Script Python que consome APIs de registro de domínios para alertar sobre novos endereços criados com o nome "Mai Wolf" (Typosquatting).
- **Análise de Logs em Tempo Real:** Automação que lê logs do Nginx e identifica picos de acesso em rotas `/login` vindos de IPs suspeitos, com integração ao SIEM.
- **Validação de MFA:** Script para auditar contas no Salesforce ou Google Workspace que ainda não possuem MFA obrigatório ativado.

### 5.2. Plano de Ação – Quick Wins (30 dias)

- **MFA Obrigatório:** Implementação em todos os níveis de acesso.
- **Gerenciadores de Senha:** Redução do risco de inserção de senhas em sites falsos, pois a ferramenta não reconhece URLs fraudulentas.
- **Honeytokens:** Inserção de credenciais falsas em pontos estratégicos; caso um script Python detecte o uso dessas credenciais, um alerta de invasão é disparado imediatamente.

---

## 6. Plano de Resposta a Incidentes (NIST Simplificado)

Modelo de resposta rápida baseado no NIST:

- **Detecção:** Alerta via Slack disparado pelo script de monitoramento de logs.
- **Contenção:** Automação para bloqueio do IP malicioso no WAF ou Firewall ao detectar brute-force ou phishing.
- **Recuperação:** Reset de credenciais comprometidas e auditoria de tokens de sessão.

---

## 7. Conclusão

A segurança moderna exige que o erro humano seja previsto e mitigado por camadas tecnológicas. A combinação de conscientização do usuário com a automação via scripts em Python posiciona a **Mai Wolf S/A** em um patamar proativo de defesa, assegurando a continuidade do negócio e a proteção de dados.
