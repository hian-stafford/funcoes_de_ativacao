# Funções de Ativação para Redes Neurais

## 📌 Descrição
Este repositório contém implementações das principais funções de ativação utilizadas em redes neurais. As funções são implementadas em Python, utilizando `numpy`, e são acompanhadas de gráficos para melhor compreensão de seu comportamento.

## 🚀 Funcionalidades
- Implementação das seguintes funções de ativação:
  - Função Degrau (Step Function)
  - Função Sigmoide (Sigmoid)
  - Função Tangente Hiperbólica (Tanh)
  - Função ReLU (Rectified Linear Unit)
  - Função Linear
  - Função Softmax
- Geração de gráficos ilustrativos
- Exemplos de uso com `numpy`

## 🛠 Tecnologias Utilizadas
- Python 3+
- Numpy
- Matplotlib (para visualização dos gráficos)

- ## 📊 Exemplos de Gráficos
### Exemplo: Função Sigmoide
```python
import numpy as np
import matplotlib.pyplot as plt

def sigmoid(x):
    return 1 / (1 + np.exp(-x))

# Exemplo de uso
x = 0.5
result = sigmoid(x)
print(f'Resultado da função sigmoide para x = 0.5: {result}')

# Criando uma lista de valores x no intervalo [0, 1]
x_values = np.linspace(0, 1, 100)

# Aplicando a função sigmoide aos valores de x
y_values = sigmoid(x_values * 10 - 5)  # Ajustando a escala para ver a transição completa de 0 a 1

# Plotando o gráfico
plt.figure(figsize=(8, 6))
plt.plot(x_values, y_values, label='Função Sigmoide', color='black', linewidth=2)
plt.title('Gráfico da Função Sigmoide')
plt.xlabel('x')
plt.ylabel('y')
plt.grid(True)
plt.legend()
plt.show()
```

## 🤝 Contribuição
Sinta-se à vontade para abrir issues e pull requests para melhorias!
