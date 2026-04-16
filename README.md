<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/1fb69f9b-60db-440a-94cc-4aa580aff9c1

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

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
}
