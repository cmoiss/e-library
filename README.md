# 📚 E-Library - Biblioteca Virtual  

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=spring&logoColor=white)](https://spring.io/)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![H2 Database](https://img.shields.io/badge/H2_Database-1F6FEB?style=flat&logo=h2&logoColor=white)]()
[![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)](https://git-scm.com/)
[![Status](https://img.shields.io/badge/STATUS-CONCLUÍDO-brightgreen)](https://github.com/cmoiss/biblioteca)
[![Licença](https://img.shields.io/badge/LICENÇA-MIT-blue)](https://opensource.org/licenses/MIT)

Sistema de biblioteca virtual desenvolvido como projeto acadêmico, permitindo empréstimos digitais, gestão de acervo e recomendações personalizadas.

---

## 🏗️ Arquitetura do Sistema

![image](https://github.com/user-attachments/assets/0c9e72b5-ee6c-462c-8431-3fa76e81bd10)


### 🔍 Componentes Principais
1. **Cliente (Frontend)**
   - Aplicação web responsiva (Next.js + Tailwind CSS)
   - Funcionalidades:
     - Busca de livros
     - Solicitação de empréstimos
     - Acompanhamento de prazos e multas
     - Avaliação de livros

2. **API (Backend)**
   - RESTful API (Spring Boot)
   - Responsável por:
     - Lógica de negócios
     - Gestão de empréstimos
     - Cálculo de multas
     - Geração de relatórios

3. **Banco de Dados**
   - H2 Database (persistência em disco)
   - Armazena:
     - Catálogo de livros
     - Registros de usuários
     - Histórico de transações

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
- Node.js 16+
- Java JDK 17+
- Maven 3.8+
- Git

### Instalação
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/e-library.git
   cd e-library
   ```

2. **Backend (Spring Boot)**
   ```bash
   cd backend
   mvn spring-boot:run
   ```

3. **Frontend (Next.js)**
   ```bash
   cd frontend
   npm install
   npm run dev
   ```

4. Acesse:
   - Frontend: `http://localhost:3000`
   - API Docs: `http://localhost:8080/swagger-ui.html`

---

## 📌 Funcionalidades Principais

### Para Clientes
- ✅ Busca avançada de livros (título, autor, ISBN)
- ✅ Empréstimo virtual com prazo calculado automaticamente
- ✅ Painel de controle com livros emprestados
- ✅ Sistema de avaliação (like/dislike)
- ✅ Recomendações personalizadas

### Para Administradores
- 🔒 CRUD completo de livros e exemplares
- 📊 Geração de relatórios (empréstimos, devoluções)
- 👥 Gerenciamento de usuários
- ⏰ Configuração de prazos e multas

---

## 🛠️ Tecnologias Utilizadas

| Área         | Tecnologias                                                                 |
|--------------|-----------------------------------------------------------------------------|
| **Frontend** | Next.js, Tailwind CSS, Axios, React Hook Form                               |
| **Backend**  | Spring Boot, JPA/Hibernate, Lombok               |
| **Banco**    | H2 Database (dev)                                     |
| **Testes**   | JUnit, Mockito                                     |
| **Outros**   | Git, Postman                                               |

---

## 📂 Estrutura do Projeto

```
e-library/
├── backend/               # Código Spring Boot
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   ├── controller/   # Endpoints REST
│   │   │   │   ├── model/        # Entidades JPA
│   │   │   │   ├── repository/   # Interfaces DAO
│   │   │   │   ├── service/      # Lógica de negócio
│   │   │   │   └── dto/          # Objetos de transferência
│   │   │   └── resources/        # application.properties
│   │   └── test/                 # Testes unitários/integração
│   └── pom.xml
│
├── frontend/              # Aplicação Next.js
│   ├── app/               # Páginas da aplicação
│   ├── components/        # Componentes React
│   ├── services/          # Chamadas à API
│   └── package.json
│
├── docs/                  # Documentação
└── README.md              # Este arquivo
```

---

## ✨ Equipe

| Função               | Integrantes                          |
|----------------------|--------------------------------------|
| **Tech Lead**        | [Caio Souza](https://github.com/cmoiss) |
| **Scrum Master**     | Rodolfo Ribeiro                      |
| **Frontend**         | Caio e [Breno Eduardo (@br3idk)](https://github.com/br3idk)      |
| **Design**           | [Nycolas Justino (@nyckturbina)](https://github.com/nyckturbina)                              |
| **Backend**          | Caio, [Igor Vinícius (@Igorzon1)](https://github.com/Igorzon1), [William Carvalho (@WillzCarvalho)](https://github.com/WillzCarvalho), [Matheus Rondon (@matheusrv0)](https://github.com/matheusrv0)         |
| **Testes**           | Caio, [Gabriel Patrício (@H4RDZ1N)](https://github.com/H4RDZ1N), Nycolas               |



---

> "Projeto desenvolvido como parte da disciplina Engenharia de Software, demonstrando na prática conceitos de desenvolvimento fullstack, gestão de projetos e trabalho em equipe." *(Atualizado em Jun/2025)*
