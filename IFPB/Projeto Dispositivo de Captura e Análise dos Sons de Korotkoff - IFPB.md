### **Projeto: Dispositivo de Captura e Análise dos Sons de Korotkoff - IFPB**

#### **1. Introdução**

Este projeto busca desenvolver um dispositivo acessível e eficiente para a **captura e análise dos sons de Korotkoff**, utilizados na medição da pressão arterial. A inovação está na **integração com um aplicativo móvel**, permitindo o armazenamento e análise dos dados em tempo real, facilitando diagnósticos médicos e contribuindo para a **prevenção de doenças cardiovasculares**.

A implementação dessa tecnologia pode beneficiar o **Sistema Único de Saúde (SUS)**, oferecendo um método não invasivo para avaliar a saúde dos vasos sanguíneos, identificando **riscos de hipertensão e doenças circulatórias** de forma **rápida e acessível**.

#### **2. Captura dos Sons de Korotkoff**

Para garantir um dispositivo eficiente, foram consideradas as seguintes melhorias: ✅ **Captura de sons com maior precisão**, filtrando ruídos externos. ✅ **Conexão com aplicativo móvel** para análise dos dados em tempo real. ✅ **Mecanismos avançados de redução de ruídos** causados por movimentação do paciente.

#### **3. Componentes Utilizados**

Os materiais necessários para a fabricação do dispositivo incluem:

|**Item**|**Função**|
|---|---|
|**Módulo de som LM393**|Captura os sons de Korotkoff|
|**Arduino Uno**|Processamento dos dados|
|**Cabo USB**|Transferência dos dados para celular|
|**Caixa Adaptadora**|Proteção dos componentes internos|
|**Estetoscópio**|Melhor captação dos sons|
|**Módulo Bluetooth HC-05**|Envio de dados para o aplicativo|

#### **4. Implementação do Sistema**

O sistema funciona da seguinte forma: 📌 **Captação dos sons**: O microfone do LM393 é integrado ao estetoscópio para eliminar interferências externas. 📌 **Processamento**: O **Arduino** ajusta a sensibilidade do módulo de som e processa os dados. 📌 **Transmissão para celular**: Os dados são enviados via **Bluetooth** para um aplicativo móvel. 📌 **Exibição dos resultados**: No aplicativo, os sons são analisados e comparados a padrões médicos para **identificação de anomalias circulatórias**.

#### **5. Desenvolvimento do Aplicativo Móvel**

O **aplicativo** receberá os dados do dispositivo e permitirá: 📱 **Monitoramento em tempo real** dos sons de Korotkoff. 📱 **Armazenamento de registros históricos** para acompanhamento médico. 📱 **Envio dos dados para profissionais de saúde** do **SUS**, melhorando diagnósticos. 📱 **Integração com IA** para sugerir possíveis condições cardiovasculares.

#### **6. Estimativa de Custo**

O custo total para a fabricação do dispositivo foi estimado conforme a tabela abaixo:

|**Item**|**Custo Unitário**|
|---|---|
|**Módulo LM393**|R$ 35,00|
|**Arduino Uno**|R$ 70,00|
|**Bluetooth HC-05**|R$ 40,00|
|**Estetoscópio**|R$ 60,00|
|**Caixa Adaptadora**|R$ 25,00|
|**Cabos e conectores**|R$ 30,00|
|**TOTAL APROXIMADO**|**R$ 260,00**|

O custo pode ser **reduzido** com produção em larga escala, tornando o dispositivo **altamente acessível para o SUS**.

#### **7. Impacto para o SUS e Saúde Pública**

💡 **Diagnóstico rápido e acessível**: O dispositivo possibilita a identificação precoce de **hipertensão e problemas circulatórios**. 💡 **Redução de custos no SUS**: Métodos tradicionais de avaliação vascular são caros. O dispositivo é uma opção **acessível** e **não invasiva**. 💡 **Facilidade de uso**: Médicos e profissionais de saúde poderão utilizar o dispositivo em **postos de saúde e unidades móveis**, beneficiando **comunidades carentes**. 💡 **Monitoramento remoto**: Pacientes podem monitorar sua pressão arterial em casa e **compartilhar dados** com médicos do SUS via aplicativo.

#### **8. Melhorias Futuras**

🚀 **IA para análise preditiva** da saúde cardiovascular. 🚀 **Expansão para hospitais e clínicas públicas**. 🚀 **Integração com prontuários médicos eletrônicos do SUS**.

Esse projeto pode transformar a maneira como **a pressão arterial é monitorada no Brasil**, garantindo **acessibilidade, inovação e suporte ao SUS**! 🎯🚀