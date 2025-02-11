# Controle de um servo motor com PWM

Este projeto implementa o controle de um servo motor utilizando o pwm na raspberry pi pico w

## Requisitos do Projeto

- **Microcontrolador**: Raspberry Pi Pico W
- **Servo Motor**
- **Led**
- **Resistor**
- **Ambiente de desenvolvimento**: VS Code + Pico SDK  
- **Simulação**: Wokwi integrada ao VS Code  

## Descrição do Funcionamento

1. O **servo motor** inicia na posição de **0°**.  
2. Ele se move para **90°** e aguarda **5 segundos**.  
3. Depois, se move para **180°** e aguarda **5 segundos**.  
4. Vai para **0°** e aguarda **5 segundos**.  
5. Após isso, o servo começa a **movimentação suave** entre **0° e 180°**, com incrementos de **5** a cada **10ms**.  
6. **Experimento adicional**: O LED RGB na **GPIO 12** é controlado por PWM para demonstrar o efeito da variação do Duty Cycle através da intensidade (Implementado na branch ledBitdoglab, mas basta alterar o pino 22 para 12).  

## Instruções de Uso

1. **Clone o repositório**:
    ```sh
    git clone https://github.com/yuriccosta/pwm_servomotor
    cd https://github.com/yuriccosta/pwm_servomotor
    ```

2. **Configure o ambiente de desenvolvimento**:
    - Instale a extensão do vscode: Raspberry Pi Pico e configure o ambiente conforme instruções.
    - Instale a extensão do vscode: Wokwi e configure o ambiente conforme instruções.

3. **Compile o código**:
    - Abra o projeto no VS Code.
    - Aperte no botão Compile da extensão do Pico SDK.

4. **Rode no wokwi integrado ao vscode**:
    - Abra o arquivo diagram.json.
    - Aperte no botão Run da extensão do Wokwi.

5. **Executando o código**:
    - O Servo motor irá funcionar conforme descrito
    - Caso esteja na branch ledBitdoglab o LED azul irá funcionar de forma semelhante com o servo motor, porém alterando a intensidade da luz emitida, ao invés de movimentar a pá.

## Vídeo de Demonstração
Assista à demonstração do projeto em execução:  
[Vídeo Demonstrativo](https://youtu.be/XfV4eqXrQLk)  
  
  
