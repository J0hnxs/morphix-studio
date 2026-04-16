<div align="center">

<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />

  <h1>Built with AI Studio</h2>

  <p>The fastest path from prompt to production with Gemini.</p>

  <a href="https://aistudio.google.com/apps">Start building</a>

</div>

# 🚀 Morphix Studio | Full-Stack Neumorphism Engine

**Morphix Studio** é uma plataforma avançada de design system para a criação de interfaces baseadas na tendência **Neumorphism (Soft UI)**. O projeto evoluiu de um gerador estático para um ecossistema completo com autenticação, persistência em nuvem e animações de alta performance.

Este projeto demonstra a integração entre o **Google AI Studio** (ambiente de desenvolvimento e refinamento) e o **Firebase** (infraestrutura de backend).

---

### 🌟 Diferenciais do Projeto
* **Ecossistema Google Cloud:** Desenvolvido e orquestrado via Google AI Studio, integrado diretamente ao Firebase.
* **Persistência Real-Time:** Diferente de outros geradores, o Morphix permite que usuários autenticados salvem suas configurações de design no **Firestore**.
* **UX Dinâmica:** Interface construída com **React 19** e **Framer Motion**, garantindo transições suaves entre estados de sombra e cor.
* **Arquitetura Profissional:** Separação clara entre lógica de UI, gerenciamento de estado e serviços de backend (Firebase Auth/Database).

---

### 🛠️ Stack Técnica
* **Frontend:** React 19 (Vite), Tailwind CSS 4.
* **Animações:** Framer Motion (`motion/react`).
* **Backend & Auth:** Firebase SDK v10 (Google Login & Firestore).
* **Ambiente de Desenvolvimento:** Google AI Studio.

---

### 🚀 Funcionalidades Implementadas
1.  **Motor de Renderização Neumórfica:** Algoritmo customizado para cálculo de sombras (`lightShadow` e `darkShadow`) baseado na luminância da cor escolhida.
2.  **Painel de Controle de Precisão:** Ajustes finos de raio, distância, intensidade e desfoque com feedback visual instantâneo.
3.  **Sistema de Autenticação:** Login social via Google totalmente integrado.
4.  **Cloud Saving:** Armazenamento de documentos JSON no banco de dados NoSQL (Firestore) com um clique.
5.  **Interface Glassmorphism:** Header moderno com efeito de desfoque de fundo (backdrop-filter) que se adapta à cor base.

---

### 📂 Como rodar o projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/morphix-studio.git](https://github.com/seu-usuario/morphix-studio.git)
    ```

2.  **Configure o Firebase:**
    Substitua o objeto `firebaseConfig` no arquivo de configuração pelas suas chaves do projeto no Firebase Console.

3.  **Instale as dependências:**
    ```bash
    npm install
    ```

4.  **Inicie o servidor de desenvolvimento:**
    ```bash
    npm run dev
    ```

---

### 🔐 Regras de Segurança (Firestore)
Para o correto funcionamento do salvamento, certifique-se de que as regras do seu Firestore permitem escrita para usuários autenticados:

```javascript
service cloud.firestore {
  match /databases/{database}/documents {
    match /designs/{design} {
      allow read, write: if request.auth != null;
    }
  }
}
