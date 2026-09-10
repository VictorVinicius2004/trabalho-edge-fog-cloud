# Trabalho de Redes sem Fio

- Pâmella ferreira de castro

- Thalles Kenedy Oliveira Maia

- Victor Vincius Figueiredo Silva

## ## Dispositivos adicionados

### 1. Sensor de fumaça/gás (`sensor_fumaca_gas`)

- **O que gera:**  `1`(fumaça/gás detectado) com 15% de chance, ou `0`
- **O que faz na decisão:** se detectado, simula uma ação crítica autônoma —
  fechar o registro de gás, ligar o exaustor e disparar o alarme local.

### 2. Painel solar (`painel_solar`)

- **O que gera:** valor de geração entre 0.0 e 4.2 kW
- **O que faz na decisão:** se a geração ultrapassa 3.0 kW, direciona o
  excedente para a bateria residencial.

### 3. Sensor de umidade do solo (`sensor_umidade_solo`)

- **O que gera:** percentual de umidade entre 15% e 80%
- **O que faz na decisão:** se a umidade cai abaixo de 22%, aciona a bomba de
  irrigação do jardim automaticamente.

### 4. Termostato de cômodo (`termostato_comodo`)

- **O que gera:** temperatura simulada entre 18°C e 35°C
- **O que faz na decisão:** se a temperatura ultrapassa 29°C, ajusta o
  ar-condicionado.

### 5. camera facial (`camera_facial`)

- **O que gera:** `"reconhecido"` ou `"nao_reconhecido"` (chance dividida em 50/50)
- **O que faz na decisão:** combinado com o sensor de janela, se uma pessoa não identificada quebrar a janela, aciona o alerta de invasão.

### 6. Sensor de janela (`sensor_janela`)

- **O que gera:** `"quebrada"` (2% de chance) ou `"normal"`
- **O que faz na decisão:** combinado com a câmera facial, se uma pessoa não identificada quebrar a janela, aciona o alerta de invasão.
