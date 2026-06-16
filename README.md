# 🔢 Gerador de CPF em Python

Projeto em Python que gera um número de CPF válido automaticamente, utilizando o algoritmo oficial de cálculo dos dígitos verificadores.

---

## 📌 Como funciona

1. Gera 9 dígitos aleatórios
2. Calcula o primeiro dígito verificador com pesos decrescentes (10 a 2)
3. Calcula o segundo dígito verificador com pesos decrescentes (11 a 2)
4. Exibe o CPF completo com 11 dígitos

---

## 🚀 Como usar

### Pré-requisitos

- Python 3.x instalado

### Execução

1. Clone o repositório:
```bash
git clone https://github.com/gelane-dev/gerador-de-cpf.git
cd gerador-de-cpf
```

2. Execute:
```bash
python gerador_cpf.py
```

### Exemplo de saída

```
76195271764
```

---

## 🧠 Lógica do algoritmo

```
9 dígitos aleatórios:  7  6  1  9  5  2  7  1  7
                       ×  ×  ×  ×  ×  ×  ×  ×  ×
                      10  9  8  7  6  5  4  3  2
                      ──────────────────────────
                      soma → (soma × 10) % 11 → 1º dígito verificador

Em seguida, repete com pesos 11→2 para o 2º dígito.
```

---

## ⚠️ Aviso

Os CPFs gerados são matematicamente válidos, mas **não pertencem a nenhuma pessoa real**. Use apenas para fins de estudo e testes.
