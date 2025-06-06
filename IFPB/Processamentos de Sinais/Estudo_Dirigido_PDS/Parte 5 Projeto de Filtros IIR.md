# **Capítulo 8: Projeto de Filtros IIR**

## **1. Introdução aos Filtros IIR**

Os **Filtros de Resposta ao Impulso Infinita (IIR)** são amplamente utilizados no processamento de sinais digitais devido à sua eficiência em atender especificações com ordens menores em comparação aos filtros FIR. Diferente dos filtros FIR, os filtros IIR possuem realimentação, o que resulta em uma resposta ao impulso infinita.

Os filtros IIR são projetados a partir de **prototipagem analógica**, onde um filtro analógico é convertido para um sistema digital equivalente. Os métodos mais comuns incluem: ✅ **Transformação bilinear** – Mapeia um filtro analógico para o domínio digital. ✅ **Aproximação de Butterworth, Chebyshev e Elíptico** – Técnicas para otimizar a resposta em frequência. ✅ **Projeto baseado em polos e zeros** – Ajuste da função de transferência para atender requisitos específicos.

## **2. Características dos Filtros IIR**

Os filtros IIR apresentam vantagens e desafios: ✅ **Alta eficiência** – Atendem especificações com ordens menores. ✅ **Menor consumo computacional** – Requerem menos coeficientes para implementação. ✅ **Resposta de fase não linear** – Pode causar distorção em algumas aplicações. ✅ **Possibilidade de instabilidade** – Deve-se garantir que todos os polos estejam dentro do círculo unitário.

A equação geral de um filtro IIR é dada por:

y[n]=∑k=0Mb[k]x[n−k]−∑j=1Na[j]y[n−j]y[n] = \sum_{k=0}^{M} b[k] x[n-k] - \sum_{j=1}^{N} a[j] y[n-j]

onde:

- y[n]y[n] é a saída do filtro.
    
- b[k]b[k] são os coeficientes do numerador.
    
- a[j]a[j] são os coeficientes do denominador.
    
- x[n−k]x[n-k] são os valores da entrada deslocados no tempo.
    

## **3. Métodos de Projeto de Filtros IIR**

### **3.1. Filtros Butterworth**

Os filtros **Butterworth** são conhecidos por sua resposta de magnitude suave e sem ondulações na banda de passagem. São ideais para aplicações onde uma transição gradual entre bandas é desejada.

### **3.2. Filtros Chebyshev**

Os filtros **Chebyshev Tipo I e II** apresentam ondulações na banda de passagem ou rejeição, permitindo uma transição mais abrupta entre bandas.

### **3.3. Filtros Elípticos**

Os filtros **Elípticos** oferecem a transição mais rápida entre bandas, mas apresentam ondulações tanto na banda de passagem quanto na banda de rejeição.

### **3.4. Transformação Bilinear**

A **Transformação Bilinear** é um método que converte filtros analógicos para digitais, garantindo que a resposta em frequência seja preservada.

## **4. Implementação Computacional**

A implementação de filtros IIR pode ser feita em **Python** e **MATLAB**. Aqui está um exemplo de um filtro Butterworth usando **SciPy** em Python:

python

```
import numpy as np
import scipy.signal as signal
import matplotlib.pyplot as plt

# Definição dos parâmetros do filtro Butterworth
order = 4
cutoff_freq = 0.3  # Frequência de corte normalizada
b, a = signal.butter(order, cutoff_freq)

# Resposta em frequência do filtro
w, h = signal.freqz(b, a)

plt.plot(w / np.pi, 20 * np.log10(abs(h)))
plt.title("Resposta em Frequência do Filtro Butterworth")
plt.xlabel("Frequência Normalizada")
plt.ylabel("Magnitude (dB)")
plt.grid()
plt.show()
```

Esse código cria um **filtro Butterworth** e exibe sua resposta em frequência.

## **5. Aplicações dos Filtros IIR**

Os filtros IIR são amplamente utilizados em: ✅ **Processamento de áudio** – Equalização e remoção de ruídos. ✅ **Processamento de imagens** – Realce de bordas e filtragem adaptativa. ✅ **Comunicações digitais** – Modulação e demodulação de sinais. ✅ **Sistemas biomédicos** – Filtragem de sinais ECG e EEG.