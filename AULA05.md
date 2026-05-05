# 📊 Análise de Refinamento de Prompts

## 1. Geração de Código

### 🔹 Prompt vago
"Crie um código em Python para calcular a soma de números."

### 🔻 Resultado típico
```python
def soma(lista):
    return sum(lista)

🔹 Prompt refinado

Código que:

recebe lista de inteiros
valida lista vazia
inclui comentários

def calcular_soma(numeros):
    # Verifica se a lista está vazia
    if not numeros:
        return 0

    soma = 0

    # Itera sobre os números e acumula o valor
    for numero in numeros:
        soma += numero

    return soma

✅ Ganho
Mais seguro (validação)
Mais didático
Melhor para manutenção

2. Refatoração de Código
🔹 Prompt vago

"Melhore este código."

🔻 Problema
Ambíguo
Sem critério de melhoria

🔹 Prompt refinado
Legibilidade
Eficiência
Boas práticas
Explicação

✅ Ganho
Código mais limpo
Melhor nomeação
Explicação das mudanças → aprendizado real

3. Documentação Técnica

🔹 Prompt vago

"Explique este código."

🔻 Problema

Explicação superficial
Sem estrutura

🔹 Prompt refinado

Estrutura:

Objetivo
Funções
Exemplos

✅ Ganho
Organização mental
Facilita onboarding
Mais aplicável no mundo real

| Critério             | Java                | Python          |
| -------------------- | ------------------- | --------------- |
| Paradigma            | Orientado a objetos | Multi-paradigma |
| Desempenho           | Alto                | Médio           |
| Curva de aprendizado | Mais difícil        | Mais fácil      |
| Uso corporativo      | Muito forte         | Crescente       |

✅ Ganho
Visual claro
Comparação direta
Melhor tomada de decisão

5. Testes Automatizados
🔹 Prompt vago

"Crie um teste para este código."

🔻 Problema
Não define ferramenta
Não define cenários
🔹 Prompt refinado
Biblioteca unittest
Casos:
lista vazia
valores negativos

import unittest

def calcular_media(lista):
    if not lista:
        return 0
    return sum(lista) / len(lista)

class TestMedia(unittest.TestCase):

    def test_lista_normal(self):
        self.assertEqual(calcular_media([2, 4, 6]), 4)

    def test_lista_vazia(self):
        self.assertEqual(calcular_media([]), 0)

    def test_valores_negativos(self):
        self.assertEqual(calcular_media([-2, -4]), -3)

if __name__ == "__main__":
    unittest.main()

CONCLUSÃO GERAL:

| Elemento   | Impacto                   |
| ---------- | ------------------------- |
| Contexto   | Evita respostas genéricas |
| Restrições | Aumenta precisão          |
| Formato    | Melhora usabilidade       |
| Papel      | Ajusta profundidade       |



