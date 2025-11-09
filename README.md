# 🧪 Sprint 4 - Testes Automatizados | MOTTU API

## 👥 Equipe

| Nome | RM |
|------|-----|
| Francesco Monteiro Di Benedetto | 557313 |
| Luiz Felipe Campos da Silva | 555591 |
| Samuel Patrick Yariwake | 556461 |

---

## 📋 Sobre

Testes automatizados para a API REST do projeto MOTTU Challenge usando **Postman**.

**API:** https://wa-challenge-mottu.azurewebsites.net

---

## 🧪 Test Cases

- **CRUD Filial** (5 requests)
- **CRUD Patio** (5 requests)
- **Listar Filiais com Patios** (1 request)
- **Listar Patios com Receptores WiFi** (1 request)

**Total:** 4 casos de teste | 12 requests | ~36 assertions

---

## 🚀 Como Executar

1. Importe `MOTTU_API_-_Sprint_4_QA.postman_collection.json` no Postman
2. Configure environment com variável `baseUrl`: `https://wa-challenge-mottu.azurewebsites.net`
3. Execute os testes via Collection Runner

---

## ⚠️ Nota sobre os Testes

Durante a execução dos testes, identificamos uma limitação no endpoint **GET /api/v1/PatioApi/{id}**:

- O endpoint retorna dados **apenas para o ID 1**
- Outros IDs (2, 3, 10, etc.) retornam **404 Not Found**
- Todos os pátios aparecem corretamente no **GET all** (listar todos)

**Impacto:** O teste READ Patio Criado pode falhar ao buscar o pátio recém-criado por ID.

---

## 🔗 Links

### Azure Boards
**Link:** [https://dev.azure.com/RM5573130642/2TDSPV-CHALLENGE](https://dev.azure.com/RM5573130642/2TDSPV-CHALLENGE)

### Vídeo Demonstrativo
**Link:** [https://youtu.be/mD-PvhLKo60](https://youtu.be/mD-PvhLKo60)

O vídeo demonstra:
- Execução dos 4 test cases
- Análise dos resultados

**Duração:** 1m44s

---

## 📁 Arquivos

```
Sprint-4-Compliance-QA/
├── README.md
└── MOTTU_API_-_Sprint_4_QA.postman_collection.json
```
