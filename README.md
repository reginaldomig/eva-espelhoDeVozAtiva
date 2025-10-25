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
- [MPSP – Pacto Ninguém se Cala](https://www.mpsp.mp.br/pacto-ninguem-se-cala)  
- [Cartilha oficial do Pacto (PDF)](https://www.al.sp.gov.br/arquivos/transparencia/pacto_ninguem_se_cala.pdf)

> 🔎 **Nota:** As fontes acima foram verificadas em **25/10/2025** e estavam ativas e atualizadas nessa data. Mudanças podem ter ocorrido desde então nos sites institucionais.

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

## 📚 Fontes oficiais e referências

- [MPSP – Pacto Ninguém se Cala](https://www.mpsp.mp.br/pacto-ninguem-se-cala)  
- [Cartilha oficial – Pacto Ninguém se Cala (PDF)](https://www.al.sp.gov.br/arquivos/transparencia/pacto_ninguem_se_cala.pdf)  
- [Ligue 180 – Central de Atendimento à Mulher](https://www.gov.br/mulheres/pt-br/ligue180)  
- [Serviço – Denunciar e buscar ajuda a vítimas de violência](https://www.gov.br/pt-br/servicos/denunciar-e-buscar-ajuda-a-vitimas-de-violencia-contra-mulheres)

> 🔎 **Fontes verificadas em 25/10/2025.** Alterações nos sites oficiais podem ocorrer com o tempo.

---

> “Ninguém se cala — porque toda voz importa.”
