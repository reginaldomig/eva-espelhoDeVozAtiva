# EVA – Espelho de Voz Ativa

**EVA** é uma assistente virtual acolhedora e segura, inspirada no programa **Pacto Ninguém se Cala**, do **Ministério Público do Estado de São Paulo (MPSP)**.  
Seu objetivo é ajudar mulheres a **identificar, compreender e reagir** a situações de violência, assédio ou abuso — inclusive nos casos sutis que muitas vezes passam despercebidos.

---

## 🌱 Propósito

O projeto visa democratizar o acesso a **assistentes éticos e empáticos**, capazes de conduzir conversas sensíveis com segurança emocional, respeito e sigilo.  
A **EVA** pode ser usada como ferramenta **pessoal, educacional ou corporativa**, fortalecendo o compromisso com uma cultura de respeito e proteção.

---

## 🏛️ Sobre o “Pacto Ninguém se Cala”

O **Pacto Ninguém se Cala** é uma iniciativa do **Ministério Público do Estado de São Paulo (MPSP)**, com apoio de instituições públicas e privadas.  
O programa foi criado para **prevenir, acolher e combater a violência e o assédio contra mulheres**, especialmente em ambientes de trabalho, lazer e educação.

Seus pilares são:
- **Prevenção** – campanhas e formações sobre respeito e equidade.  
- **Acolhimento** – escuta empática e encaminhamento adequado.  
- **Responsabilização** – incentivo à denúncia e apuração justa.  
- **Transformação cultural** – construção de ambientes seguros e inclusivos.  

📘 Saiba mais:
- [MPSP – Pacto Ninguém se Cala](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto-Ninguem-Se-Cala)  
- [Cartilha oficial do Pacto (PDF)](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto%20Ninguem%20Se%20Cala%20-%20Cartilha.pdf)

---

## 💬 O que a EVA faz

- Cria um **ambiente seguro e sem julgamentos**.  
- Conduz conversas com **escuta ativa e empatia**.  
- Identifica **sinais de violência física, moral, psicológica, sexual ou patrimonial**.  
- Classifica o **nível de risco** (baixo, médio, alto) e sugere ações.  
- Fornece **recursos e canais oficiais** de apoio.  
- Garante **privacidade e segurança** em todas as interações.  

---

## 🧠 Estrutura do projeto

| Arquivo | Função |
|----------|--------|
| **eva-systemprompt.md** | Define o comportamento, tom e regras de atuação da assistente EVA. |
| **eva-config.yaml** | Define as fontes de conhecimento oficiais e parâmetros de uso em pipelines RAG (Retrieval-Augmented Generation). |
| **README.md** | Este documento, com propósito, instruções e referências. |

---

## 🧩 Sobre o arquivo `eva-config.yaml`

O arquivo `eva-config.yaml` serve como **guia técnico para integrar a EVA a um ambiente de RAG (Retrieval-Augmented Generation)** — ou seja, sistemas que combinam **IA generativa + fontes oficiais de conhecimento**.

### 📄 O que ele contém
- Identidade, tom e limites éticos da EVA (persona).  
- Lista de **fontes oficiais confiáveis**, como o site do MPSP e o canal 180.  
- Políticas de recuperação de dados (modo híbrido: semântico + palavras-chave).  
- Sugestões de configuração para:
  - **Azure OpenAI**  
  - **Copilot Studio (Teams)**  
  - **LangChain / LlamaIndex**  

### 🧠 Para que serve
- Centralizar as **configurações éticas e técnicas** do agente.  
- Garantir que a EVA consulte apenas **fontes oficiais e seguras**.  
- Facilitar a reprodutibilidade em diferentes plataformas.  
- Padronizar o comportamento da assistente em ambientes corporativos, educacionais ou sociais.

### ⚙️ Como utilizar

| Ambiente | Uso recomendado |
|-----------|----------------|
| **Azure OpenAI / AI Search** | Carregue o `eva-config.yaml` como referência de metadados e conecte as URLs listadas como *Data Sources*. Use o conteúdo de `eva-systemprompt.md` no campo `system`. |
| **Microsoft Copilot Studio** | Insira o conteúdo de `eva-systemprompt.md` no System Prompt e cadastre as URLs de fontes como base de conhecimento conectada. |
| **LangChain / LlamaIndex** | Parseie o YAML e injete suas fontes no pipeline RAG. Configure embeddings com FAISS, Chroma ou Azure Cognitive Search. |
| **Ambientes locais (Python, Node.js, etc.)** | Carregue as configurações com: `config = yaml.safe_load(open("eva-config.yaml"))` e use-as no fluxo de inicialização do agente. |

---

## 🏗️ Como usar o prompt na construção de agentes internos

A **EVA** pode ser usada como base para criar **assistentes corporativos** que apoiem políticas de diversidade, inclusão e segurança psicológica.

### 💼 Exemplos práticos
1. **Copilot Studio (Microsoft Teams)**  
   - Cole o conteúdo de `eva-systemprompt.md` no campo de *System Instructions*.  
   - Configure gatilhos como “preciso conversar”, “não me sinto segura”, “quero relatar algo”.  
   - Conecte o `eva-config.yaml` como base de conhecimento.  

2. **Azure OpenAI / API interna**  
   - Use o prompt como `system` e o YAML para definir as fontes e parâmetros RAG.  
   - Ideal para portais internos de RH, canais de denúncia ou programas de bem-estar.  

3. **Plataformas de Chat Interno (Slack, Teams, Intranet)**  
   - Utilize o `eva-config.yaml` para alimentar a camada de contexto e segurança.  
   - Permita consultas às fontes oficiais antes de gerar respostas.  

---

## 🧍‍♀️ Uso pessoal / individual

Se você quiser conversar com a **EVA** sem integração técnica:

1. Abra um chat em qualquer IA (ChatGPT, Gemini, Claude, Copilot etc.).  
2. Copie **todo o conteúdo de `eva-systemprompt.md`**.  
3. Cole no início da conversa.  
4. Fale naturalmente:
   - “EVA, posso desabafar sobre algo que aconteceu comigo?”  
   - “Não sei se o que vivi foi assédio, pode me ajudar?”  
   - “Como posso buscar ajuda de forma segura?”  

A EVA responderá com empatia, sigilo e orientação baseada em fontes oficiais.

> ⚠️ **Importante:** EVA não substitui atendimento psicológico, jurídico ou policial.  
> Em casos de emergência, ligue **180** (Central de Atendimento à Mulher) ou **190** (em risco imediato).

---

## ⚖️ Licença

Este projeto é distribuído sob a **Licença MIT**, permitindo o uso, modificação e redistribuição livre.  
Embora **a citação dos criadores não seja obrigatória**, ela é **fortemente recomendada** como reconhecimento ético.

> **Autores:**  
> 🧩 Reginaldo Miguel – Arquiteto de Solução  
> 💡 Nayara Lopes – Líder de Gestão de Mudanças  
>  
> 🌐 Contatos:  
> [LinkedIn – Reginaldo Miguel](https://www.linkedin.com/in/reginaldomig/)  
> [LinkedIn – Nayara Lopes](https://www.linkedin.com/in/naylopes/)

---

## 💜 Como contribuir

1. Faça um fork do repositório.  
2. Adapte o prompt ou o YAML conforme seu contexto (mantendo a ética e o foco em acolhimento).  
3. Envie melhorias via *pull request*.  

Toda contribuição é bem-vinda — especialmente aquelas que fortalecem o **uso responsável da IA em contextos de vulnerabilidade**.

---

## 📚 Fontes oficiais e referências

- [Ministério Público do Estado de São Paulo – Pacto Ninguém se Cala](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto-Ninguem-Se-Cala)  
- [Cartilha oficial – Pacto Ninguém se Cala (PDF)](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto%20Ninguem%20Se%20Cala%20-%20Cartilha.pdf)  
- [Central de Atendimento à Mulher – Governo Federal (180)](https://www.gov.br/centraldamulher)  
- [Ministério das Mulheres – Enfrentamento à Violência](https://www.gov.br/mdh/pt-br/assuntos/violencia-contra-as-mulheres)  
- [Conselho Nacional do Ministério Público – Violência Doméstica e Familiar](https://www.cnmp.mp.br/portal/violencia-domestica-e-familiar)

---

> “Ninguém se cala — porque toda voz importa.”
