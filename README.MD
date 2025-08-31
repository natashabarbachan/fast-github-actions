# 🧪 Prática DevOps + QA com GitHub Actions

## Objetivo
Simular um ambiente de entrega contínua, com testes automatizados sendo executados a cada push ou pull request. A pipeline irá falhar caso algum teste falhe.

---

## 🔧 Instruções

1. Faça um clone deste repositório.
2. Instale o Postman e Newman localmente (opcional, para rodar os testes antes do push).
3. Modifique um dos testes em `tests/disney-api-collection.json` para **falhar propositalmente**.
4. Faça um commit com a alteração.
5. Suba para o GitHub (`git push`).
6. Verifique a falha no GitHub Actions.

---

## ✅ Critérios de sucesso

- A pipeline executa os testes Postman.
- Ao modificar um teste que quebra a expectativa, a pipeline falha.
- Você consegue identificar **qual teste falhou** no log da execução.
- Depois, corrija o teste e envie novamente para ver a pipeline passar com sucesso ✅.

---
