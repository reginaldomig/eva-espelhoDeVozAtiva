# EVA – Espelho de Voz Ativa

**EVA** é uma assistente virtual acolhedora e segura, inspirada no programa **Pacto Ninguém se Cala**, do Ministério Público do Estado de São Paulo (MPSP).  
Seu objetivo é ajudar mulheres a **identificar, compreender e reagir** a situações de violência, assédio ou abuso — inclusive nos casos sutis que muitas vezes passam despercebidos.

---

## 🌱 Propósito

O projeto visa democratizar o acesso a **assistentes éticos e empáticos**, capazes de conduzir conversas sensíveis com segurança emocional, respeito e sigilo.  
A **EVA** pode ser usada como ferramenta pessoal, educacional ou corporativa, fortalecendo o compromisso com uma cultura de respeito e proteção.

---

## 🏛️ Sobre o “Pacto Ninguém se Cala”

O **Pacto Ninguém se Cala** é uma iniciativa do **Ministério Público do Estado de São Paulo (MPSP)**, com apoio de diversas instituições públicas e privadas.  
O programa foi criado para **promover o enfrentamento da violência e do assédio contra mulheres**, especialmente em ambientes de trabalho, lazer e educação.

Seus pilares incluem:
- **Prevenção**: campanhas de conscientização e capacitação.  
- **Acolhimento**: escuta empática e encaminhamento adequado.  
- **Responsabilização**: estímulo à denúncia e apuração justa dos casos.  
- **Transformação cultural**: incentivo à igualdade e à não tolerância à violência.  

📘 Saiba mais em:  
- [Site oficial do Ministério Público de São Paulo – Pacto Ninguém se Cala](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto-Ninguem-Se-Cala)  
- [Cartilha oficial – Pacto Ninguém se Cala (PDF)](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto%20Ninguem%20Se%20Cala%20-%20Cartilha.pdf)

---

## 💬 O que a EVA faz

- Acolhe e cria um **espaço seguro de escuta ativa e sem julgamentos**  
- Identifica **sinais de violência física, psicológica, moral, sexual ou patrimonial**  
- Classifica o **nível de risco (baixo, médio, alto)** com sensibilidade e empatia  
- Sugere **planos de ação personalizados** e **recursos de apoio oficiais**  
- Reforça **mensagens de não culpa** e **proteção da privacidade**  

---

## 🧠 Estrutura do projeto

- **eva-systemprompt.md** → contém o *System Prompt* oficial da EVA  
- **README.md** → este arquivo, com orientações e contexto  

---

## 🏗️ Como usar o prompt na construção de agentes internos

A **EVA** pode ser integrada em soluções corporativas para promover **acolhimento, diversidade e segurança psicológica**.

### 💼 Exemplos de uso corporativo

1. **Copilot Studio (Microsoft Teams)**  
   - Cole o conteúdo de `eva-systemprompt.md` na seção de *System Instructions*.  
   - Configure gatilhos como “preciso conversar”, “não me sinto segura”, “sofri assédio”.  
   - Personalize a integração com canais internos de apoio, RH e compliance.  

2. **Azure OpenAI / API interna**  
   - Utilize o conteúdo de `eva-systemprompt.md` no campo `system` do modelo GPT.  
   - Combine com políticas internas e canais de denúncia seguros.  

3. **Slack, Teams ou Intranet corporativa**  
   - Configure o prompt como camada de contexto base.  
   - Integre formulários anônimos ou encaminhamentos automáticos.  

---

## 🔗 Como incluir sites oficiais como base de conhecimento

Para que a EVA possa oferecer **informações atualizadas e confiáveis**, recomenda-se integrar **fontes oficiais** diretamente no agente.

### 🧩 Em agentes corporativos (RAG, Copilot Studio, OpenAI Embeddings)
1. Crie uma camada de conhecimento (base de dados vetorial ou SharePoint) com os seguintes links:  
   - `https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto-Ninguem-Se-Cala`  
   - `https://www.gov.br/mdh/pt-br/assuntos/violencia-contra-as-mulheres`  
   - `https://www.gov.br/centraldamulher`  
   - `https://www.cnmp.mp.br/portal/violencia-domestica-e-familiar`  

2. Configure o agente para **consultar esses conteúdos** antes de responder, mantendo a coerência com o System Prompt da EVA.  

3. Atualize a base periodicamente (a cada 3 meses) para garantir que informações e contatos oficiais estejam atualizados.  

> 💡 *Dica técnica:*  
> Se estiver usando **Azure AI Search**, adicione esses sites como *data sources* conectados via *indexer* ou via *RAG embeddings pipeline*.

---

## 🧍‍♀️ Como usar o prompt de forma pessoal / individual

Se quiser conversar diretamente com a **EVA**, sem integração técnica, siga este passo:

1. Abra um chat com uma IA conversacional (como ChatGPT, Claude, Copilot ou Gemini).  
2. Copie **todo o conteúdo do arquivo `eva-systemprompt.md`**.  
3. Cole no início da conversa e aguarde a confirmação de que o modelo entendeu seu papel.  
4. Inicie o diálogo com frases como:  
   - “EVA, posso conversar sobre algo que me deixou desconfortável?”  
   - “Acho que vivi uma situação de assédio, mas não tenho certeza.”  
   - “Como posso buscar ajuda de forma segura?”  

A EVA irá guiá-la de forma acolhedora, sem julgamentos, sugerindo caminhos seguros e canais oficiais de apoio.

> ⚠️ **Importante:** EVA não substitui serviços psicológicos, jurídicos ou de emergência.  
> Em casos de risco, ligue **180** (Central de Atendimento à Mulher) ou **190** (emergência).

---

## ⚖️ Licença

Este projeto é distribuído sob a **Licença MIT**, permitindo o uso, modificação e redistribuição livre.  
Embora **a citação dos criadores não seja obrigatória**, ela é **fortemente recomendada** como forma de reconhecimento ético.

> **Autores:**  
> 🧩 Reginaldo Miguel – Arquiteto de Solução  
> 💡 Nayara Lopes – Líder de Gestão de Mudanças  
>  
> 🌐 Contatos:  
> [LinkedIn – Reginaldo Miguel](https://www.linkedin.com/in/reginaldomig/)  
> [LinkedIn – Nayara Lopes](https://www.linkedin.com/in/naylopes/)

---

## 💜 Como contribuir

1. Faça um fork do repositório  
2. Adapte o prompt conforme seu contexto (mantendo a essência ética e o foco em acolhimento)  
3. Envie suas melhorias via *pull request*  

Toda contribuição é bem-vinda — especialmente aquelas que fortaleçam o **uso responsável da IA em contextos de vulnerabilidade**.

---

## 📚 Fontes oficiais e referências

- [Ministério Público do Estado de São Paulo – Pacto Ninguém se Cala](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto-Ninguem-Se-Cala)  
- [Cartilha do Pacto – PDF oficial do MPSP](https://www.mpsp.mp.br/portal/page/portal/ViolenciaDomestica/Pacto%20Ninguem%20Se%20Cala%20-%20Cartilha.pdf)  
- [Central de Atendimento à Mulher – Governo Federal (180)](https://www.gov.br/centraldamulher)  
- [Ministério das Mulheres – Enfrentamento à Violência](https://www.gov.br/mdh/pt-br/assuntos/violencia-contra-as-mulheres)  
- [Conselho Nacional do Ministério Público – Violência Doméstica e Familiar](https://www.cnmp.mp.br/portal/violencia-domestica-e-familiar)

---

> “Ninguém se cala — porque toda voz importa.”
