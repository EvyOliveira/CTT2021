# Lista de Exercícios XIII

> À partir do dia 12 de março. A aula referente à essa Lista de Exercícios foi sobre design de API, boas práticas de modelagem de APIs. 

```js

// Seguindo o uso correto dos métodos HTTP, devemos utilizar o método GET para qual finalidade?
[x] Recuperar dados.
[] Salvar dados.
[] Substituir dados.
[] Atualizar dados.

// Seguindo o uso correto dos métodos HTTP, devemos utilizar o método PATCH para qual finalidade?
[] Recuperar dados.
[] Salvar dados.
[] Substituir dados.
[x] Atualizar dados.

// Métodos HTTP idempotentes são métodos capazes de:
[] Fazer a requisição sem alterar o estado do recurso (em sucesso).
[x] Fazer várias vezes a mesma requisição obtendo o mesmo retorno (em sucessos).
[] São métodos capazes de fazer requisições, mas gerando efeito colateral.
[] Recuperar sem alteração de estado informações previamente armazenadas. 

// Métodos HTTP seguros são métodos capazes de:
[x] Fazer a requisição sem alterar o estado do recurso (em sucesso).
[] Fazer várias vezes a mesma requisição obtendo o mesmo retorno (em sucessos).
[] São métodos capazes de fazer requisições, mas gerando efeito colateral.
[x] Recuperar sem alteração de estado informações previamente armazenadas. 

// Qual desses métodos HTTP é seguro?
[x] GET.
[] PUT.
[] PATCH.
[] DELETE.

// Qual desses métodos HTTP NÂO é idempotente?
[] GET.
[] PUT.
[x] PATCH.
[] DELETE.

// Qual destes exemplos segue as recomendações de como definir recursos?
[] /Estudantes.
[] /estudante.
[] /obter-estudantes.
[x] /estudantes/{id}/notas.

// Qual destes exemplos segue as recomendações de como definir recursos?
Definição de plural. Recomendável estar.
[] /criarOrdensVenda.
[] /ordensVenda.
[x] /ordens-venda.
[] /ordem-venda.

// Sobre métodos HTTP de sucesso x recursos, qual(is) status code(s) é(são) recomenda(s) no retorno de GET/estudantes?
[] 201.
[] 200 ou 204.
[x] 200 ou 206.
[] 202.

// Sobre métodos HTTP de sucesso x recursos, qual(is) status code(s) é(são) recomenda(s) no retorno de POST/estudantes/1?
Definindo um id no estudante do recurso, teríamos que definir um elemento do post. Nesse caso, criaríamos um regostro na base com ele.
[] 201.
[] 200.
[] 400.
[x] 405.

// Sobre recomendações de versionamento, quais desses casos o versionamento é recomendado (múltiplas respostas):
Sempre causa impacto quando você restringe a API, quando aceitava uma representação e não aceita mais.
[x] Remover alguma funcionalidade. 
[] Inserção de um novo atributo opcional.
[] Passar a aceitar mais um tipo de representação (sem alteração da default).
[x] Passar a não aceitar mais tipo de representação.

// Quais das URIs abaixo segue as recomendações de design de APIs:
[] https://api.qa.sensedia.com/financas/1.0.2/pagamentos. 
[x] https://api.qa.sensedia.com/financas/v1/pagamentos.
[] https://api.sensedia.com/qa/financas/v1/pagamentos.
[] https://api.qa.sensedia.com/financas/v1/pagamento.

```
