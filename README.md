# Projeto Final: Integração Contínua e Entrega Contínua (CI/CD)

Este repositório contém a aplicação prática desenvolvida para o curso **Integração Contínua e Entrega Contínua (CI/CD)** oferecido pela IBM no Coursera. O projeto demonstra a aplicação de conceitos de DevOps através de pipelines automatizadas de CI e CD.

## 🚀 Status do Projeto (Badges)
Abaixo está o indicador em tempo real da nossa pipeline de Integração Contínua:

![CI Workflow](https://github.com)

---

## 📦 Sobre a Aplicação
A aplicação consiste em um microsserviço desenvolvido em **Python/Flask** (ou a tecnologia do seu lab) que expõe endpoints de uma API Rest funcional.

### Funcionalidades:
- Endpoint de verificação de integridade (`/health`)
- Gerenciamento de recursos da API

---

## 🛠️ Arquitetura de CI/CD

O projeto foi automatizado utilizando duas abordagens complementares:

1. **Integração Contínua (CI) - GitHub Actions:**
   - Executada a cada `push` ou `pull request` na branch `main`.
   - Realiza o linting do código para garantir padrões de estilo (`flake8`).
   - Executa a suite de testes unitários automaticamente (`pytest` ou `green`).

2. **Entrega Contínua (CD) - Tekton / OpenShift:**
   - Pipeline de CD que constrói a imagem Docker da aplicação.
   - Publica a imagem no container registry.
   - Realiza o deploy automatizado no cluster Kubernetes/OpenShift.

---

## 💻 Como Executar Localmente

### Pré-requisitos
- Python 3.x instalado
- Git

### Passo a Passo
1. Clone o repositório:
   ```bash
   git clone https://github.com
   cd NOME_DO_REPOSITORIO
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

3. Execute os testes manualmente:
   ```bash
   pytest
   ```

4. Inicie o servidor de desenvolvimento:
   ```bash
   python server.py
   ```

---

## 👥 Autor
- **Seu Nome** - [Seu Perfil do GitHub](https://github.com)
- Projeto desenvolvido como parte do Certificado Profissional de DevOps da IBM.
