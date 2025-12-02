# Projeto_Final_CyberSec_VNW---Pishing---
Projeto Final - VNW - CyberSec - Mai Wolf S/A

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/c0dfbf53-4519-4d87-8f32-67a1b201f116" />

# Relatório de Simulação de Engenharia Social 

**Cliente:** Mai Wolf S/A 

**Setor:** Redes Sociais

**Elaborado por:** Maiara Viegas – Analista de Segurança 

**Data:** 30/11/2025  

---
## 1. Sumário Executivo

Foi realizada uma simulação simples de ataque de Engenharia Social com foco em **phishing**, utilizando um ambiente controlado. O objetivo foi demonstrar como uma página falsa pode se parecer com uma página legítima e induzir um usuário iniciante a fornecer credenciais.

A técnica usada foi a de **captura de credenciais**. A página falsa tinha aparência semelhante ao site original, demonstrando como usuários desatentos podem ser enganados facilmente.

**Principais riscos identificados:**

- Semelhança visual entre página verdadeira e falsa.  
- Falta de verificação da URL antes de inserir dados.  
- Exposição de credenciais ao acessar sites falsos.

---

## 2. Metodologia e Escopo

A simulação teve caráter educacional e buscou demonstrar conceitos básicos de phishing e engenharia social, com foco no entendimento do comportamento humano.

**Escopo incluído:**

- Criação de uma página fictícia para captura de credenciais de teste.  
- Demonstração da interação da vítima simulada com o site falso.  
- Observação dos erros cometidos no processo.

**Observação:**  
Nenhuma credencial real foi usada,assim como nenhum usuário real foi envolvido.

---

## 3. Descrição da Simulação

### 3.1. Configuração Inicial

Foi montado um ambiente seguro para a atividade. Em seguida, foi criada uma página de login falsa com visual semelhante à página legítima, contendo campos básicos para e-mail e senha.

### 3.2. Página Falsa para Coleta de Dados

A página simulada replicava a estrutura visual de um site de login comum. O objetivo era apenas demonstrar como o phishing funciona na prática.

### 3.3. Acesso da Vítima (Simulada)

Durante a simulação:

- A vítima fictícia acessou o endereço utilizado no laboratório.  
- A página parecia legítima, então ela inseriu as credenciais de teste.  
- Os dados foram capturados imediatamente no ambiente de simulação.  

Isso demonstrou como um ataque básico pode ter sucesso quando o usuário não faz a validação de segurança.

---

## 4. Análise de Risco Humano

| Fator | Descrição |
|-------|-----------|
| **Confiança no visual** | A página falsa era semelhante à original, o que gerou confiança. |
| **Não verificação da URL** | Esse foi o principal erro que permitiu o sucesso do phishing. |
| **Familiaridade com o serviço** | Usuários tendem a confiar em sites conhecidos apenas pelo visual, sem verificar detalhes técnicos. |

A simulação destacou a importância do comportamento do usuário na prevenção de ataques.

---

## 5. Conclusão e Recomendações

A simulação demonstrou que **o maior ponto fraco em ataques de phishing é o comportamento humano**. Mesmo ataques simples podem ser eficazes quando o usuário não verifica o endereço antes de digitar suas informações.

### Recomendações para usuários iniciantes

- **Sempre conferir a URL** antes de inserir credenciais.  
- **Evitar clicar em links inesperados**, especialmente solicitando login.  
- **Ativar autenticação multifator (MFA)** para impedir acesso mesmo quando a senha é comprometida.  
- **Utilizar gerenciadores de senhas**, que preenchem credenciais somente em sites legítimos.  
- **Participar de treinamentos de conscientização** sobre phishing e ameaças básicas.  

Essas práticas reduzem significativamente o risco de exposição a ataques de engenharia social.

---

