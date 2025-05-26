# **Capítulo 7: Projeto de Filtros FIR**

## **1. Introdução aos Filtros FIR**

Os **Filtros de Resposta ao Impulso Finita (FIR)** são amplamente utilizados no processamento de sinais digitais devido à sua estabilidade e resposta de fase linear. Diferente dos filtros **IIR (Infinite Impulse Response)**, os filtros FIR possuem uma resposta ao impulso finita, tornando-os ideais para aplicações onde a preservação da fase do sinal é essencial.

Os filtros FIR são projetados a partir da **convolução discreta** e podem ser implementados por diferentes métodos, como: ✅ **Método das Janelas** – Aplicação de uma janela para truncar a resposta ao impulso. ✅ **Aproximação de Parks-McClellan** – Algoritmo de otimização baseado na equiripple. ✅ **Transformação de frequência** – Modificação de filtros existentes para novas especificações.

## **2. Características dos Filtros FIR**

Os filtros FIR apresentam vantagens significativas: ✅ **Estabilidade garantida** – Como não possuem realimentação, são sempre estáveis. ✅ **Resposta de fase linear** – Essencial para aplicações em áudio e comunicações. ✅ **Facilidade de implementação** – Podem ser projetados diretamente a partir da resposta ao impulso desejada.

A equação geral de um filtro FIR é dada por:

y[n]=∑k=0Mh[k]x[n−k]y[n] = \sum_{k=0}^{M} h[k] x[n-k]

onde:

- y[n]y[n] é a saída do filtro.
    
- h[k]h[k] são os coeficientes do filtro.
    
- x[n−k]x[n-k] são os valores da entrada deslocados no tempo.
    

## **3. Métodos de Projeto de Filtros FIR**

### **3.1. Método das Janelas**

O **Método das Janelas** é uma abordagem simples para projetar filtros FIR. Ele consiste em: 1️⃣ Definir um **filtro ideal** no domínio da frequência. 2️⃣ Aplicar uma **janela** para truncar a resposta ao impulso. 3️⃣ Ajustar os coeficientes para minimizar efeitos indesejados.

As janelas mais comuns incluem: ✅ **Janela Retangular** – Simples, mas com alta dispersão espectral. ✅ **Janela de Hamming** – Reduz efeitos de Gibbs, melhorando a resposta. ✅ **Janela de Blackman** – Excelente supressão de lóbulos secundários.

### **3.2. Algoritmo de Parks-McClellan**

O **Algoritmo de Parks-McClellan** é um método avançado baseado na otimização equiripple. Ele ajusta os coeficientes do filtro para minimizar o erro entre a resposta ideal e a projetada.

### **3.3. Transformação de Frequência**

A **Transformação de Frequência** permite modificar filtros existentes para atender novas especificações. Esse método é útil para converter filtros passa-baixa em passa-alta, passa-faixa ou rejeita-faixa.

## **4. Implementação Computacional**

A implementação de filtros FIR pode ser feita em **Python** e **MATLAB**. Aqui está um exemplo de um filtro FIR usando **SciPy** em Python:

python

```
import numpy as np
import scipy.signal as signal
import matplotlib.pyplot as plt

# Definição dos coeficientes do filtro FIR
num_taps = 51
cutoff_freq = 0.3  # Frequência de corte normalizada
fir_coeffs = signal.firwin(num_taps, cutoff_freq)

# Resposta em frequência do filtro
w, h = signal.freqz(fir_coeffs)

plt.plot(w / np.pi, 20 * np.log10(abs(h)))
plt.title("Resposta em Frequência do Filtro FIR")
plt.xlabel("Frequência Normalizada")
plt.ylabel("Magnitude (dB)")
plt.grid()
plt.show()
```

Esse código cria um **filtro FIR** e exibe sua resposta em frequência.

## **5. Aplicações dos Filtros FIR**

Os filtros FIR são amplamente utilizados em: ✅ **Processamento de áudio** – Equalização e remoção de ruídos. ✅ **Processamento de imagens** – Suavização e detecção de bordas. ✅ **Comunicações digitais** – Modulação e demodulação de sinais. ✅ **Sistemas biomédicos** – Filtragem de sinais ECG e EEG.