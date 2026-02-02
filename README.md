cat <<EOF > README.md
# 🍃 Eventify API 

[![Java](https://img.shields.io/badge/Java-17%2B-orange?style=for-the-badge&logo=java)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.2-brightgreen?style=for-the-badge&logo=spring-boot)](https://spring.io/projects/spring-boot)
[![JWT](https://img.shields.io/badge/JWT-Authentication-black?style=for-the-badge&logo=json-web-tokens)](https://jwt.io/)

### 📝 Sobre o Projeto
O **Eventify** é uma API robusta para gerenciamento de eventos técnicos. Este projeto foi concebido como um **"Laboratório de Backend"** para aplicar e documentar as melhores práticas do ecossistema Java moderno, focando especialmente em segurança, performance e código limpo.

---

### 🛠️ Tecnologias e Implementações

* **Core:** Java 17+ e Spring Boot 3.
* **Segurança:** Autenticação Stateless com **JWT (JSON Web Token)** e controle de acesso via **Roles** (ADMIN/USER).
* **Criptografia:** Implementação de \`BCryptPasswordEncoder\` para proteção de credenciais.
* **Manipulação de Dados:** Uso extensivo de **Java Streams e Lambdas** para filtragem e transformação de objetos.
* **Arquitetura:** Padrão **DTO (Data Transfer Object)** para evitar exposição direta das entidades de banco de dados.
* **Documentação:** Interface interativa com **Swagger UI (OpenAPI 3)**.
* **Persistência:** Spring Data JPA com banco de dados (H2 para testes ou PostgreSQL para produção).

---

### 🗄️ Estrutura de Dados (Database Schema)
O projeto conta com 4 tabelas principais com relacionamentos complexos:
1.  **Users:** Gestão de acesso e perfis.
2.  **Events:** Informações detalhadas sobre os eventos disponíveis.
3.  **Categories:** Classificações (ex: Java, Cloud, DevOps).
4.  **Tickets:** Vínculo entre usuários e eventos (Inscrições).

---

### 🚀 Como Rodar a Aplicação

1. **Clone o repositório:**
   \`\`\`bash
   git clone https://github.com/SEU-USUARIO/eventify-api.git
   \`\`\`
2. **Configure o Banco:** O projeto utiliza H2 por padrão.
3. **Execute:**
   \`\`\`bash
   ./mvnw spring-boot:run
   \`\`\`
4. **Documentação:** Acesse \`http://localhost:8080/swagger-ui.html\`

---
💻 Desenvolvido para centralizar estudos no Notion.
EOF
