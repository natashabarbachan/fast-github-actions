# 🧪 Prática DevOps + QA com GitHub Actions

## Objetivo
Simular um ambiente de entrega contínua, com testes automatizados sendo executados a cada push ou pull request. A pipeline irá falhar caso algum teste falhe.

---

## 🔧 Instruções

1. Faça um clone deste repositório.  
2. Crie uma branch nova a partir da `main` para realizar suas alterações:  
   ```bash
   git checkout -b minha-branch
   ```
3. Instale o Postman e Newman localmente (opcional, para rodar os testes antes do push).  
4. Modifique um dos testes em `tests/disney-api-collection.json` (por exemplo, para falhar propositalmente).  
5. Faça um commit das suas alterações:  
   ```bash
   git add .
   git commit -m "Descrição das alterações"
   ```
6. Suba sua branch para o GitHub:  
   ```bash
   git push origin minha-branch
   ```
7. Abra um **Pull Request (PR)** da sua branch para a `main`.  
8. Aguarde a execução da pipeline do GitHub Actions e verifique se **todos os status checks passam**.  
9. Somente quando os checks passarem e o PR for aprovado, sua branch poderá ser mergeada na `main`. Se algum teste falhar, o merge será bloqueado até a correção.

---

## ✅ Critérios de sucesso

- A pipeline executa os testes Postman.  
- Ao modificar um teste que quebra a expectativa, a pipeline falha.  
- Você consegue identificar **qual teste falhou** no log da execução.  
- Depois, corrija o teste e envie novamente para ver a pipeline passar com sucesso ✅.
