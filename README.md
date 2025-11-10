# Prova CI — Logan Moraes

Este repositório contém um projeto simples em TypeScript configurado com um pipeline de Integração Contínua (CI) utilizando GitHub Actions.  
O objetivo é demonstrar um fluxo automatizado de instalação, testes e build.

---

## ✅ Como rodar o projeto localmente

### Instalar dependências:

```bash
npm install
```

### Rodar testes:

```bash
npm test
```

### Gerar build:

```bash
npm run build
```

---

## ✅ Estrutura do Projeto

src/ → código-fonte TypeScript
tests/ → testes unitários com Jest
.github/workflows/ci.yml → pipeline CI

---

## ✅ Explicação do Pipeline CI

O workflow `ci.yml` é executado automaticamente quando há:

- Push na branch **main**
- Pull request direcionado à **main**

Etapas executadas:

1. **Checkout do repositório**
2. **Instalação das dependências (npm install)**
3. **Execução dos testes automatizados (npm test)**
4. **Build (npm run build)**

Caso qualquer etapa falhe, o GitHub marca o status como **failed**, garantindo controle de qualidade contínuo.

---

## ✅ Testes

Foi utilizado Jest para criar dois testes simples da função `soma`, validando:

- Soma básica  
- Soma com número negativo  

Isso demonstra o funcionamento do pipeline de testes.
